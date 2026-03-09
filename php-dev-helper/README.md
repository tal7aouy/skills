# PHP Development Assistant (build & scaffold tool)

A language‑specific assistant for PHP, CodeIgniter, and Laravel projects.
It helps you write code faster by generating boilerplate, suggesting
clearer structures, and flagging common framework pitfalls.

### Who it’s for

- **PHP developers** building web applications
- **Engineers using CodeIgniter or Laravel** who want consistent output
- **Teams** that appreciate automated scaffolding and style checks

This tool is a productivity companion; it does _not_ replace manual
review or reading the official docs.

## Example usage

```bash
# run a full analysis on the repository
/php-dev-helper

# include a deeper adversarial check
/php-dev-helper deep

# analyze only certain files
/php-dev-helper app/Models/User.php

# generate a new controller
/php-dev-helper generate controller User

# save the report to assets/reports
/php-dev-helper --file-output
```

The command works the same way in the VS Code Claude extension or in
Cursor.

> ⚠️ Suggestions are AI‑generated; validate them before committing.
