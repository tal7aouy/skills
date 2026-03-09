# Laravel/PHP Development Assistant

A CLAUDE‑powered assistant for Laravel engineers. Use it to generate
controllers, migrations and routes, get suggestions about Eloquent usage,
middleware, and to avoid common mistakes while building your app.

Designed for:

- **Laravel developers** building web applications
- **PHP engineers** who want quick scaffolding and advice
- **Teams** enforcing consistent patterns across projects

This tool is a convenience layer over LLMs; it is not a replacement for
reading the official documentation or performing code reviews.

## Usage

```bash
# Analyze the repository
/laravel-dev-helper

# Run a deeper, adversarial review
/laravel-dev-helper deep

# Inspect particular files or folders
/laravel-dev-helper app/Http/Controllers/UserController.php

# Generate boilerplate
/laravel-dev-helper generate controller User

# Save results to disk
/laravel-dev-helper --file-output
```

Parameters are the same when invoked from the VS Code Claude extension or
when using Cursor.

## Notes

- The skill ignores `vendor/`, `node_modules/`, `tests/`, and similar
  vendored directories by default.
- Reports and generated files go under `assets/reports/` when
  `--file-output` is supplied.

> ⚠️ AI suggestions are just that; always verify generated code and
> review analysis manually.
