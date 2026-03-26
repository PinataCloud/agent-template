# Useful Assistant — OpenClaw Agent Template

A general-purpose personal assistant template for OpenClaw. Ships with a complete workspace structure, personality framework, and memory system.

## What You Get

- **A personal assistant that bootstraps itself** — on first run, it introduces itself and figures out who it is with you
- **Memory system** — daily logs + curated long-term memory that persists across sessions
- **Personality framework** — SOUL.md defines who the agent is, evolves over time
- **Heartbeat support** — periodic check-ins for email, calendar, and proactive work

## Structure

```
manifest.json                # Agent config, secrets, and all available options documented
workspace/
  BOOTSTRAP.md               # First-run conversation guide (self-deletes after setup)
  SOUL.md                    # Agent personality and principles
  AGENTS.md                  # Workspace conventions, memory system, safety rules
  IDENTITY.md                # Agent name, vibe, emoji (filled in during bootstrap)
  USER.md                    # Notes about the human (learned over time)
  TOOLS.md                   # Environment-specific notes (cameras, SSH, TTS, etc.)
  HEARTBEAT.md               # Periodic tasks (empty by default)
```

## Manifest Options

The `manifest.json` includes a `_docs` section documenting every available field:

- **agent** — name, description, vibe, emoji
- **model** — default AI model
- **secrets** — encrypted API keys and credentials
- **skills** — attachable skill packages from ClawHub
- **tasks** — cron-scheduled prompts
- **routes** — port forwarding for web apps/APIs
- **channels** — Telegram, Discord, Slack configuration
- **template** — marketplace listing metadata

Remove the `_docs` block before submitting to the marketplace.

## Usage

Import this repo when creating an agent on [Pinata Agents](https://agents.pinata.cloud).
