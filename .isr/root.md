# ISR — Intentional Software Representation

## Purpose
Maintain a living representation of a software system's intention, enabling LLMs to act as reasoned co-architects across sessions.

## Serves
Developers who use AI-assisted development and need to preserve design intent.

## Enables
- Consistent AI understanding across sessions without re-explanation
- Architectural coherence over time
- Reasoned decision-making aligned with original intent

## Principles
- Intention over implementation — capture the "why", not the "how"
- Recursive structure — same format at every level of detail
- Graph of nodes — no rigid hierarchy, concepts link freely
- Concise and non-redundant — no narrative documentation
- Living document — evolves with the project
- LLM as guardian — prevents drift by validating actions against intent

## Boundaries
- Does: Capture intent, principles, constraints, concept relationships
- Does NOT: Replace code, duplicate implementation details, prescribe step-by-step specs

## Relations
- node — the fundamental building block
- index — enables navigation
- directive — guides LLM behavior
- bootstrapping — handles existing projects
