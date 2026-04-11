# Railyard KB Plugin

A Claude Code plugin for managing the Railyard Knowledge Base lifecycle and enforcing KB-driven development.

## Commands

| Command | Description |
|---------|-------------|
| `/kb:new [domain/scope]` | Create a new KB article (interactive or `--quick`) |
| `/kb:update <path>` | Refresh an article to match current code |
| `/kb:audit [domain]` | Find codebase features not covered by the KB |
| `/kb:lint [domain]` | Run health checks on KB consistency |
| `/kb:stale [domain]` | Find articles whose source code has changed |
| `/kb:gaps [path]` | List and manage gap files |

## Skills

- **kb-enforcement** — Auto-triggers on code tasks to load relevant KB articles, check gap files, and warn about staleness
- **kb-conventions** — Shared article format rules loaded by agents

## Agents

- **kb-writer** — Creates and updates KB articles
- **kb-auditor** — Runs audit and staleness checks
- **kb-linter** — Runs KB health checks

## Installation

```bash
claude plugins add /home/sean/railyard-kb-plugin
```
