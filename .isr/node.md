# Node

## Purpose
The atomic unit of intention representation — one concept, one file.

## Serves
Both humans and LLMs who need to understand a specific concept.

## Enables
- Granular navigation through the project's intent
- Isolated updates without affecting unrelated concepts
- Loading only relevant context for a given task

## Principles
- Self-contained — a node has all info needed to understand the concept
- Uniform structure — every node follows the same template
- Explicit relations — links to other nodes are declared, not implicit
- Flat storage — all nodes at same directory level (no nested folders)

## Structure
Every node contains:
```markdown
# [Concept Name]

## Purpose
[Why this exists — one sentence]

## Serves
[Who/what benefits from this]

## Enables
[What becomes possible because of this]

## Principles
[Rules specific to this concept]

## Boundaries
- Does: [responsibilities]
- Does NOT: [anti-responsibilities]

## Relations
- other_concept — nature of the link
```

## Boundaries
- Does: Represent one concept's intention completely
- Does NOT: Contain implementation details, code references, or specs

## Relations
- index — registers this node for discovery
- relation — links this node to others
