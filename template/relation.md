# Relation

## Purpose
Express a meaningful link between two concepts.

## Serves
LLMs who need to understand concept dependencies and impacts.

## Enables
- Loading related context when working on a concept
- Impact analysis when modifying a concept
- Understanding the semantic graph of the project

## Principles
- Bidirectional by convention — if A relates to B, B should mention A
- Free-form description — no controlled vocabulary, natural language
- Declared in nodes — relations live in the nodes, not in a central registry
- Minimal — only meaningful relations, not every possible link

## Structure
In a node's Relations section:
```markdown
## Relations
- other_concept — brief description of the link
```

## Boundaries
- Does: Connect concepts semantically
- Does NOT: Imply hierarchy, enforce direction, define technical dependencies

## Relations
- node — relations are declared within nodes
