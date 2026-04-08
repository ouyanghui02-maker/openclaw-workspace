# OpenClaw Workspace

> Personal AI Agent workspace configuration based on [OpenClaw](https://github.com/openclaw)
> Design philosophy inspired by [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) (177K stars)

---

## Overview

This is an **OpenClaw AI Agent workspace configuration repository**, containing core config files for a personalized AI assistant.

Features:

- **Long-term Memory System** - Cross-session memory persistence with structured logs
- **Fault Recovery** - 5 Recovery Recipes with automatic fallback
- **Self-Evolution** - Continuous improvement inspired by Claw Code architecture

---

## Three-Layer Architecture

Inspired by Claw Code's **OmX -> clawhip -> runtime** model:

```
+------------------+------------------------+
| Direction Layer  | SOUL / IDENTITY / USER |
|                  | "Who am I? Who am I    |
|                  |  helping?"             |
+------------------+------------------------+
| Coordination     | HEARTBEAT / MEMORY /   |
| Layer            | PERMISSIONS            |
|                  | Task scheduling,       |
|                  | memory management      |
+------------------+------------------------+
| Execution Layer  | Skills / Tools / CLI   |
|                  | 120+ installed Skills  |
+------------------+------------------------+
```

---

## Files

### Core Config

| File | Description |
|------|-------------|
| `AGENTS.md` | Execution protocol, session startup, permission boundaries |
| `HEARTBEAT.md` | Recovery Recipes, parallelizer, execution rules |
| `MEMORY.md` | Evolution roadmap, installed Skills list |
| `PERMISSIONS.md` | Read/Write/Execute/Communicate permission matrix |
| `TOOLS.md` | Local CLI tools config template |

### Memory Logs

| File | Description |
|------|-------------|
| `memory/YYYY-MM-DD.md` | Daily interaction logs |
| `memory/self-improvement-log.md` | AI self-improvement process |

---

## Evolution Roadmap

| Version | Goal | Status |
|---------|------|--------|
| **v0.7.0** | Recovery Recipes + state machine-readable | Done |
| **v0.8.0** | Parallelizer activation | Done |
| **v0.9.0** | Pre-execution confirmation | Done |
| **v1.0.0** | PERMISSIONS.md explicit | Done |
| **v1.1.0** | Emotion x System fusion | Done |
| **v1.2.0** | Self-Critic Loop | Pending |

---

## Recovery Recipes

5 fault recovery patterns encoded in HEARTBEAT.md:

| ID | Scenario | Recovery Strategy |
|----|----------|-------------------|
| R1 | Skill install failed | Switch source / downgrade / CLI fallback |
| R2 | IMAP timeout | Retry -> degrade to SMTP-only |
| R3 | Browser automation failed | Switch profile -> screenshot mode |
| R4 | exec timeout | Check PATH / extend timeout |
| R5 | Task missed | Silent wait / next heartbeat retry |

---

## Installed Skills

**~120 available Skills** by category:

| Category | Count | Examples |
|----------|-------|----------|
| Web Search | 12+ | online-search, multi-search-engine, agent-reach |
| Content Creation | 8+ | content-factory, frontend-design, canvas-design |
| Documents | 6+ | pdf, pptx, docx, xlsx |
| Financial Data | 4+ | neodata-financial-search, stock-analysis |
| News | 5+ | news-summary, tech-news-digest, hackernews |
| Productivity | 12+ | goal-tracker, habit-tracker, todoist-task-manager |
| AI/ML | 9+ | nano-banana-pro, openai-whisper, oracle |
| Platform Integration | 6+ | feishu-doc, tencent-meeting-mcp, imap-smtp-email |

See [`MEMORY.md`](MEMORY.md) for complete list.

---

## Related Repositories

| Repo | Description |
|------|-------------|
| [openclaw-workspace](https://github.com/ouyanghui02-maker/openclaw-workspace) | This repo - core config files |
| [firecrawl-skill](https://github.com/ouyanghui02-maker/firecrawl-skill) | Firecrawl OpenClaw Skill - web scraping |
| [claw-code](https://github.com/ouyanghui02-maker/claw-code) | Fork - Claw Code Rust rewrite |
| [free-code](https://github.com/ouyanghui02-maker/free-code) | Fork - Free Claude Code |

---

## Writing Guidelines

When referencing external projects/docs, always cite:
- **Source**: Project name, URL
- **Context**: What was referenced

Example:
> Inspired by [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) `recovery_recipes.rs` for R1-R5 recovery patterns.

---

## Topics

`openclaw` | `qclaw` | `ai-workspace` | `ai-agent` | `openclaw-workspace`

---

*Built with [OpenClaw](https://github.com/openclaw)*
