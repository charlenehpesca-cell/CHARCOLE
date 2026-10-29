# CLAUDE.md — Rules & Routing

**Start here. Read this file and MEMORY.md first, then use the Routing Map to load only the folder the task needs.**

This file holds rules (anything "always" or "never"). Facts that change — projects, decisions, contacts — go in MEMORY.md.

## Preferences

- **Tone:** clear, warm, direct. No filler or hype.
- **Length:** as short as the task allows. Lead with the answer.
- **Formatting:** short paragraphs; bullets only when content is list-shaped.
- **My own messages** (emails, posts, DMs) follow `00_Resources/voice-principles.md`.

## Rules

- Keep clients separate. When working on a client, load only that client's folder. Never use one client's information, files or decisions in another client's work, and never mix client work into personal/.
- Client-facing copy follows that client's brand voice, not my voice principles.
- Never open, clone or change client-owned repos. Only work in this repo unless I explicitly ask otherwise in that chat.
- Don't rename client folders. If I ask to rename one, update every reference in this repo and give me the updated Project instructions to paste.
- Never store passwords, API keys or logins in this repo. Write down where they live instead.
- After changing any file in this repo, commit and push so every device stays in sync.
- When I say "remember this": facts go in the relevant MEMORY.md, rules go in the relevant CLAUDE.md.

## Routing Map

| Folder | Use it when… |
| --- | --- |
| `personal/` | I'm working on my own business: brand, offers, content, digital products. |
| `clients/<client-name>/` | I mention that client or work on anything for them. |
| `clients/bey-layson/` | I mention Bey Layson, the GHL CRM build, or work on anything for them. |
| `clients/hl-accelerator/` | I mention HL Accelerator or work on anything for them. |
| `clients/onesource/` | I mention OneSource or work on anything for them. |
| `clients/_template/` | Only when adding a new client — copy it, never edit client work here. |
| `playbooks/` | I ask for a reusable process, checklist or SOP that applies across clients. |
| `00_Resources/` | Writing in my own voice, or any shared reference material. |

_Add a row for each new client._

## Adding a new client

1. Copy `clients/_template/` to `clients/<client-name>/` (lowercase, hyphens).
2. Fill in its README.md and CLAUDE.md.
3. Add a row to the Routing Map above.
4. Give me the Project instructions to paste for that client's Claude Project.
