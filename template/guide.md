# Guide

## Purpose
Explain the ISR approach to anyone discovering this folder.

## What is ISR?

ISR (Intentional Software Representation) captures the **intention** behind a software system — the "why", not the "how". It serves as a persistent semantic framework that enables LLMs to act as reasoned co-architects across sessions.

## Core Idea

One concept = one file (a **node**). Nodes link to each other through **relations**, forming a flat graph of intentions. No hierarchy, no implementation details, no code references.

## How to Use This Folder

### Starting a Session
1. Read `_index.md` — discover all concepts
2. Read `root.md` — understand the project's core intent
3. Load relevant nodes based on the task at hand

### Before Any Action
1. Identify which nodes are relevant
2. Load the node + its direct relations
3. Verify the action aligns with Purpose, Principles, Boundaries
4. If goals, concepts, or intentions are unclear → ask user to clarify BEFORE proceeding
5. If aligned → proceed
6. If ambiguous → ask user for clarification
7. If misaligned → refuse and explain why

### Maintaining ISR
- Update affected nodes when intent changes
- Add new nodes for new concepts
- Keep `_index.md` in sync
- Maintain bidirectional relations

## Node Structure

Every node follows this template:

```markdown
# [Concept Name]

## Purpose
Why this exists — one sentence.

## Serves
Who or what benefits from this.

## Enables
What becomes possible because of this.

## Principles
Rules specific to this concept.

## Boundaries
- Does: [responsibilities]
- Does NOT: [anti-responsibilities]

## Relations
- other_concept — nature of the link
```

## Key Principles

- **Intention over implementation** — capture why, not how
- **One concept per file** — atomic, self-contained nodes
- **Flat structure** — no nested folders, all nodes at same level
- **Explicit relations** — links are declared, not implicit
- **Prevention over detection** — validate before acting
- **Proactive disambiguation** — clarify unclear goals, concepts, or intentions before starting work
- **User arbitration** — never make implicit decisions
- **English canonical content** — for LLM performance

## Boundaries
- Does: Explain the ISR approach and how to use it
- Does NOT: Define the project's intent (that's root's job)

## Relations
- root — the project's entry point after reading this guide
- node — defines the structure explained here
- directive — detailed LLM behavior rules
- _index.md — the navigation file mentioned here
