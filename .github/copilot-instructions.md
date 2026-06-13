<!-- file: .github/copilot-instructions.md -->
<!-- version: 1.2.0 -->
<!-- guid: f6a7b8c9-d0e1-4234-f5a6-b7c8d9e0f1a2 -->
<!-- last-edited: 2026-06-13 -->

# gha-ci-workflow-helpers — Additional Context

Org-wide coding standards (file headers, language rules, commit format) are at
**<https://github.com/falkcorp/.github>** and apply automatically to this repo.

For full project context: **CLAUDE.md** at the repo root.

## Project overview

GHA composite action: CI workflow helper utilities. Language: YAML.

## Key directories

- `action.yml` — composite action entry point with embedded Python script
- `template/` — action templates

## Critical constraints

- All logic is embedded in `action.yml` using `shell: python` — no separate `src/` directory.
- All commits MUST use conventional commit format: `type(scope): description`.
- Always update version headers in files you modify.
