# Node/JavaScript Development Assistant (scaffolding & guidance)

A lightweight CLI assistant that uses LLM agents to help Node/JS and
Express developers build applications. It can generate boilerplate,
give stylistic and architectural suggestions, and flag common pitfalls.

Designed for:

- **Node.js/Express developers** who want quick feedback on their code
- **Full‑stack engineers** juggling multiple frameworks
- **Teams** that need consistent scaffolding of routes, controllers, and
  middleware

This tool is **not a substitute for manual review** or thorough testing,
but it’s a useful companion during everyday development.

## Usage

```bash
# Scan the full repo (default)
/node-dev-helper

# Include adversarial reasoning for deeper analysis
/node-dev-helper deep

# Review specific file(s)
/node-dev-helper src/controllers/UserController.js

# Generate a new router or controller
/node-dev-helper generate controller User

# Output results to disk instead of terminal
/node-dev-helper --file-output
```

You can also run the command from the VS Code Claude extension or
in Cursor using the same invocation.

## Notes

- It ignores vendored directories like `node_modules/`, `dist/`,
  `vendor/`, and `tests/` by default.
- Reports are produced in Markdown and can be written under
  `assets/reports/` when `--file-output` is specified.

> ⚠️ The assistant relies on AI; use its suggestions as guidance rather
> than authoritative answers.
