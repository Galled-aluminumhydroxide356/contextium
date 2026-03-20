# Codex

AI code generation agent for bulk file edits and large refactors.

## Requirements

- Codex CLI installed
- API key configured

## Setup

1. Install the Codex CLI
2. Configure your API key
3. See `agent-configs/claude/AGENTS.md` for delegation rules

## Key Commands

```bash
codex "refactor all files to use new naming convention"
codex "generate tests for src/utils/"
codex "update imports across the project"
```

## When to Delegate to Codex

- Bulk file edits across many files
- Code generation from specifications
- Large-scale refactors (renaming, restructuring)
- Repetitive edits that follow a pattern

## Use Cases

- Generating boilerplate code from templates
- Applying consistent changes across a codebase
- Creating test files for existing modules
- Migrating code between frameworks or patterns
