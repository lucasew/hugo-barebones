# Agent Instructions

This repository uses `mise` for tool management and task execution.

## Tooling

- **Mise**: Manages tools and tasks. Ensure you have `mise` installed.
- **Trunk**: Handles linting and formatting.
- **Hugo**: Static site generator.

## Tasks

Run tasks using `mise run <task>`.

- `lint`: Runs `trunk check`.
- `fmt`: Runs `trunk fmt`.
- `test`: Runs `hugo` to build the site.
- `codegen`: Updates generated code (currently empty).
- `install`: Installs dependencies (currently empty).
- `ci`: Runs `lint` and `test`.

## CI/CD

The `.github/workflows/autorelease.yml` workflow handles CI, PR creation for codegen changes, and releases.

## Development

1.  Install `mise`.
2.  Run `mise install` to install tools.
3.  Run `mise run ci` to verify changes.
