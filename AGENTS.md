# Repository Guidelines

## Project Structure & Module Organization
This repository is currently empty (no files or folders detected in the root). As you add code, keep a clear top-level layout so new contributors can orient quickly. A common, easy-to-navigate structure is:

- `src/` for application or library code
- `tests/` for automated tests
- `scripts/` for dev automation
- `assets/` for static files (images, fixtures)

If you choose a different layout, document it in this file and in `README.md`.

## Build, Test, and Development Commands
No build or test tooling is present yet. When you add a build system, list the exact commands here and in the README. Example patterns (only if applicable) include:

- `make build` for a Makefile-driven build
- `npm run dev` for a Node.js dev server
- `pytest` for a Python test suite

Keep commands deterministic and document required environment variables.

## Coding Style & Naming Conventions
No language or formatter is configured yet. Once you choose a language, specify:

- Indentation (e.g., 2 spaces for JS/TS, 4 spaces for Python).
- Naming conventions (e.g., `snake_case` for Python modules, `PascalCase` for classes).
- Formatting/lint tools (e.g., `prettier`, `ruff`, `gofmt`) and how to run them.

## Testing Guidelines
There is no testing framework configured. When tests are introduced, document:

- Frameworks (e.g., `pytest`, `jest`).
- Test naming (e.g., `test_*.py`, `*.spec.ts`).
- How to run all tests and any fast subsets.

## Commit & Pull Request Guidelines
No Git history exists yet. Once version control is initialized, pick a commit convention (for example, Conventional Commits) and document it here. For pull requests, require:

- A clear summary of changes and rationale.
- Linked issues or task references when applicable.
- Screenshots or logs for UI/behavior changes.

## Configuration & Security Notes
If secrets or local config are required, keep them in `.env` files that are excluded from version control, and provide an `.env.example` template with safe defaults.
