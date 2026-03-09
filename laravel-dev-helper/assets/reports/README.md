# Reports

**⚠️ Work in Progress — this feature is not ready yet.**

This directory holds two kinds of reports:

- **Reports from previous `/laravel-dev-helper` runs** — written automatically
  as `{project-name}-tal7aouy-ai-report-{timestamp}.md` each time the skill
  runs in an analysis mode.
- **External reports or notes** — drop any third-party or manual
  review or analysis `.md` files here, for example results from a
  security review or performance report.

On each run the skill may read every file in this directory and
re‑verify whether previously reported issues still exist in the current
code. Issues still present are carried forward with a “Previously
reported – still present” note. Issues that are no longer present are
silently skipped.

Feel free to repurpose this directory for scaffolding history or other
project‑specific notes as needed.
