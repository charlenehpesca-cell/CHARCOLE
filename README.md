# CHARCOLE — Second Brain

Private notes repo shared by Obsidian (on my computer) and Claude (on every device). Everything syncs through GitHub.

## What lives where

| Path | What's in it |
| --- | --- |
| `CLAUDE.md` | Rules, preferences and the routing map. Claude reads this first. |
| `MEMORY.md` | General facts: active projects, decisions, contacts. |
| `00_Resources/` | Shared references, including my voice principles. |
| `clients/_template/` | Copy this for every new client. |
| `clients/<name>/` | One folder per client, each with its own CLAUDE.md and MEMORY.md. |
| `personal/` | My own business: brand, offers, content, digital products. |
| `playbooks/` | Reusable processes for every client. |

## Sync

- Obsidian Git plugin: auto commit-and-sync and auto pull every 5 minutes, pull on startup.
- Instant sync in Obsidian: Cmd + P → **Git: Pull** or **Git: Commit-and-sync**.
- Fallback: GitHub Desktop → Commit to main → Push origin.

Never store passwords, API keys or tokens here.
