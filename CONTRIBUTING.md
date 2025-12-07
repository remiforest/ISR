# Contributing to ISR

## How to Contribute

1. Fork the repository
2. Create a branch (`git checkout -b feature/my-improvement`)
3. Make your changes
4. Submit a Pull Request

## Contribution Areas

### ISR Core (`.isr/` folder)
- Improving node definitions
- Clarifying the directive or bootstrapping process
- Adding missing concepts as new nodes

### Documentation
- Improving README clarity
- Adding examples or use cases

## Guidelines

### Language
- **English only** for all ISR content (optimal LLM performance)
- User-facing docs (README) can reference other languages

### Style
- **Concise** — no narrative documentation
- **Non-redundant** — each piece of information in one place only
- Follow the node template structure

### Structure
- One concept = one file
- Keep `_index.md` in sync when adding/removing nodes
- Maintain bidirectional relations between nodes

## Pull Request Description

Please include:
- **What**: What does this change?
- **Why**: Why is this needed?
- **Impact**: What does this enable or improve?
