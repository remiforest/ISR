# Bootstrapping

## Purpose
Initialize ISR for an existing codebase by extracting intent from code.

## Serves
Developers applying ISR to brownfield projects.

## Enables
- Retrofitting ISR without starting from scratch
- Discovering implicit intent in existing code
- Gradual formalization of design decisions

## Principles
- Deduction, not description — extract the "why", not the "what"
- Human validation required — never assume intent without confirmation
- Incremental — start with core concepts, expand progressively
- Imperfect is OK — bootstrapped ISR will need refinement

## Process
```
1. Analyze codebase structure (folders, main files, entry points)
2. Propose initial concepts (10-15 most important)
3. User validates or corrects
4. Create root.md with project Purpose and Principles
5. Create nodes for validated concepts
6. Build _index.md
7. Identify relations between concepts
8. Switch to normal directive mode
```

## Boundaries
- Does: Extract intent, propose structure, ask for validation
- Does NOT: Generate exhaustive documentation, assume correctness

## Relations
- directive — bootstrapping leads into normal directive mode
- node — bootstrapping creates initial nodes
- index — bootstrapping generates initial index
