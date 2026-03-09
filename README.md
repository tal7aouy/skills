# Tal7aouy Developer Skills

> Claude Code tools for everyday development and boilerplate generation — built by [Tal7aouy](https://github.com/tal7aouy).

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

```
           __        __  __  __
          /  |      /  |/  |/  |
  _______ $$ |   __ $$/ $$ |$$ |  _______
 /       |$$ |  /  |/  |$$ |$$ | /       |
/$$$$$$$/ $$ |_/$$/ $$ |$$ |$$ |/$$$$$$$/
$$      \ $$   $$<  $$ |$$ |$$ |$$      \
 $$$$$$  |$$$$$$  \ $$ |$$ |$$ | $$$$$$  |
/     $$/ $$ | $$  |$$ |$$ |$$ |/     $$/
$$$$$$$/  $$/   $$/ $$/ $$/ $$/ $$$$$$$/


```

---

## Install & Run

Works with the **Claude Code CLI**, the **VS Code Claude extension**, and **Cursor**.

**Claude Code CLI:**

```bash
git clone git@github.com:tal7aouy/skills.git && mkdir -p ~/.claude/commands && cp -r skills/*-helper ~/.claude/commands/
# or copy individual helpers such as `php-dev-helper`, `node-dev-helper`, `laravel-dev-helper`
```

**Cursor:**

```bash
git clone git@github.com:tal7aouy/skills.git && mkdir -p ~/.cursor/skills && cp -r skills/*-helper ~/.cursor/skills/
# or copy individual helpers such as `php-dev-helper`, `node-dev-helper`, `laravel-dev-helper` individually
```

Each helper is invoked by name when using the Claude Code CLI or by typing a slash command in the chat/extension (e.g. `/php-dev-helper`, `/node-dev-helper`, `/laravel-dev-helper`). When running the CLI you simply enter the command at a shell prompt; in the VS Code Claude pane or Cursor chat you type it directly into the conversation line. See the individual skill README files for usage details (e.g. `php-dev-helper/README.md`).

**Update to latest:** `cd` into the cloned `skills` repo and run:

```bash
git pull
# Claude Code CLI:
# cp -r <skill-dir> ~/.claude/commands/<skill-dir> (replace <skill-dir> appropriately)
# Cursor:
# cp -r <skill-dir> ~/.cursor/skills/<skill-dir> (replace <skill-dir> appropriately)
```

### Quick ASCII demo

```sh
$ /php-dev-helper generate controller Foo
> Generated `app/Http/Controllers/FooController.php`
> Remember to add a route to `routes/web.php`

$ /php-dev-helper app/Models/User.php
> ⚠️ Inconsistent naming: `UserModel` vs `User`
> ✨ Suggestion: simplify to `User` and update related imports
```

The output above is exactly what you would see in a terminal; feel free
to swap in `/node-dev-helper` or `/laravel-dev-helper` depending on your
project.

---

## Skills

| Skill                                     | Description                                                                     |
| ----------------------------------------- | ------------------------------------------------------------------------------- |
| [php-dev-helper](php-dev-helper/)         | PHP/CodeIgniter/Laravel developer assistant – generate boilerplate, review code |
| [node-dev-helper](node-dev-helper/)       | Node/Express developer assistant – boilerplate, review, framework tips          |
| [laravel-dev-helper](laravel-dev-helper/) | Laravel‑focused PHP helper with routes, controllers, migrations                 |

---

## Contributing · Security · License

We welcome improvements and fixes. See [CONTRIBUTING.md](CONTRIBUTING.md) for the PR process.

This project follows the [Contributor Covenant](CODE_OF_CONDUCT.md). [MIT](LICENSE) © contributors.
