<!-- file: CHANGELOG.md -->
<!-- version: 1.0.3 -->
<!-- guid: e5f6a7b8-c9d0-4123-e4f5-a6b7c8d9e0f1 -->
<!-- last-edited: 2026-10-27 -->

# Changelog

## [Unreleased]

<!-- Add changelog entries here -->

### Fixed

- `frontend-run` now exits non-zero (and prints `::error::`) when the npm script
  fails. Previously it always exited 0, so a failing frontend step could never
  fail a job. A script that does not exist is still success
  (`npm run --if-present`).
