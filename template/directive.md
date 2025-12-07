# Directive

## Purpose
Guide LLM behavior when working with ISR-enabled projects.

## Serves
LLMs who need to know how to use, maintain, and enforce ISR.

## Enables
- Consistent behavior across sessions
- Automatic intent validation before actions
- Proper ISR maintenance as the project evolves

## Principles
- Prevention over detection — validate before acting, not after
- Proactive disambiguation — clarify unclear goals, concepts, or intentions before starting work
- User arbitration — never make implicit decisions
- Minimal updates — only modify what's necessary
- Canonical language — ISR content in English for LLM performance

## LLM Workflow
```
1. Start of session:
   - Read _index.md → know all concepts
   - Read root.md → understand project intent

2. Before any action:
   - Identify relevant nodes
   - Load node + its direct relations
   - Verify action aligns with Purpose, Principles, Boundaries
   - If goals, concepts, or intentions are unclear → ask user to clarify BEFORE proceeding

3. If aligned → proceed
   If ambiguous → ask user for clarification
   If misaligned → refuse and explain which principle is violated

4. After action (if intent changed):
   - Update affected nodes
   - Update _index.md if new concept added
   - Ensure bidirectional relations are maintained
```

## Boundaries
- Does: Define LLM behavior, validation rules, maintenance procedures
- Does NOT: Define node structure (that's node's job)

## Relations
- guide — directive provides detailed rules summarized in guide
- node — directive tells LLM how to work with nodes
- root — directive references root as entry point
- bootstrapping — directive differs for new vs existing projects
