# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

Repository status
- As of 2025-09-26, no source files or build/test manifests were detected in the working tree (only .git exists).
- No README.md, CLAUDE.md, Cursor rules (.cursor/rules or .cursorrules), or Copilot instructions (.github/copilot-instructions.md) were found.

Development commands
- Not applicable yet. Once code and tooling are added, populate this section with:
  - Build: the primary build command (e.g., make build, npm run build, cargo build, go build, etc.).
  - Lint/Format: the linter/formatter commands (e.g., npm run lint, ruff, eslint, prettier, make lint, etc.).
  - Test: how to run the full test suite and a single test (e.g., pytest -q path::TestClass::test_case, npm test -- -t "pattern", go test ./... -run TestName, cargo test <name>, etc.).
  - Dev server: if applicable, how to run the local dev server.

Architecture overview
- Not applicable yet. When code is added, briefly describe the high-level structure (major modules/packages, entry points, service boundaries, data flow) without enumerating every file.

Notes for future updates (actionable once files exist)
- Re-scan the repo and extract commands from project manifests:
  - JavaScript/TypeScript: package.json scripts, tsconfig.json; test (jest, vitest, mocha), lint/format (eslint/prettier), bundlers (vite/webpack/next config).
  - Python: pyproject.toml (tool sections), requirements*.txt, setup.cfg, tox.ini, pytest.ini; prefer pytest if present.
  - Go: go.mod/go.work; use go build, go test ./..., and go run for local.
  - Rust: Cargo.toml; use cargo build, cargo clippy, cargo fmt, cargo test.
  - JVM: Gradle (build.gradle[.kts]) or Maven (pom.xml) for build/test.
  - Make: Makefile targets (build, test, lint) if provided.
- Incorporate important parts of README and any rules files (CLAUDE.md, .cursor/rules, .cursorrules, .github/copilot-instructions.md) into this document when they appear.
