<div align="center">

<img src="docs/logo.png" width="96" alt="Sakina AI Desktop logo" />

# Sakina AI Desktop

**A professional desktop workspace for AI — cloud models, your own local and LAN models, an agent that works with your files and terminal, Skills, Connectors and Plugins.**

[![Latest release](https://img.shields.io/github/v/release/imomzoda-dev/SakinaAiDesktop?label=release&color=D97757)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/total?color=D97757)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-0078d4)
![Languages](https://img.shields.io/badge/UI-English%20%7C%20Русский%20%7C%20Тоҷикӣ-6b7280)
[![License](https://img.shields.io/badge/license-EULA%20(freeware)-6b7280)](LICENSE.md)

[**⬇ Download for Windows**](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest) · [Changelog](CHANGELOG.md) · [Русский](README.ru.md)

<img src="docs/screenshots/01-chat.png" alt="Sakina AI Desktop — chat" width="900" />

</div>

---

## Why Sakina

- **Any model, one app.** OpenAI, Anthropic Claude, Google Gemini, OpenRouter, Groq, DeepSeek, Mistral, Moonshot Kimi and any OpenAI-compatible API — **plus your own models**: Ollama, Open WebUI, vLLM, SGLang, llama.cpp, LM Studio, Kimi K2 self-hosted and 20 more local/LAN servers.
- **Private by design.** No telemetry. Chats, projects and settings stay on your PC; API keys are encrypted with Windows DPAPI. Route sensitive projects to local models only.
- **An agent that really works.** Reads and edits files, runs commands in your terminal, uses Git — every risky action waits for your approval, and every step is visible in a timeline.
- **Claude-style extensibility.** Skills (SKILL.md), Connectors (MCP) and Plugins (Claude Code format) — install the most popular ones from GitHub in one click.
- **Updates itself.** New versions are found on GitHub Releases, downloaded with progress, verified (SHA-512) and installed with one click — your data stays.

## Features

| | |
|---|---|
| 💬 **Chat** | Streaming answers, Markdown, tables, code highlighting, Mermaid, HTML/SVG preview, reasoning ("thinking") blocks, attachments incl. PDF text, branching edits, search, export |
| 🧠 **Models & routing** | Cloud and local providers, multi-key rotation, live health of local servers, automatic default model, smart / privacy-first / local-only routing |
| 🖥️ **Local & LAN AI** | 28 server types with a 6-step connection test; detects Open WebUI / Ollama / OpenAI-compatible servers and fixes the address in one click |
| 🛠️ **Agent & code workspace** | File explorer, Monaco editor, PowerShell / CMD / Git Bash terminal, Git panel, task checklist, approvals for risky actions, undo of file changes |
| ✨ **Skills** | Catalog of 100 popular skills (Anthropic, obra/superpowers, addyosmani/agent-skills…), create your own, import from folder / .zip / GitHub; used automatically or with `/skill-name` |
| 🔌 **Connectors** | 19 verified MCP connectors (GitHub, Context7, DeepWiki, Microsoft Learn, Playwright, Notion, Brave Search, Supabase, Sentry…) — tokens stored encrypted |
| 🧩 **Plugins** | The official Anthropic marketplace (300+ plugins) and any GitHub marketplace in Claude Code format: skills, slash commands and connectors |
| 🧭 **Comfort** | Global hotkey `Ctrl+Shift+Space`, tray icon, command palette `Ctrl+K`, shortcuts `Ctrl+/`, drafts per chat, response styles, notifications, light/dark themes, collapsible sidebar |
| 🔒 **Safety** | Path guard, command risk analysis, permission rules, audit log, backups with SHA-256 verification, database copy before every schema upgrade |

## Screenshots

| | |
|---|---|
| <img src="docs/screenshots/02-welcome-light.png" alt="Welcome screen" /> | <img src="docs/screenshots/09-workspace.png" alt="Code workspace" /> |
| **Welcome** — light theme | **Code workspace** — editor, terminal, AI agent |
| <img src="docs/screenshots/04-skills-catalog.png" alt="Skills catalog" /> | <img src="docs/screenshots/03-skills.png" alt="My skills" /> |
| **Skills catalog** — 100 popular skills from GitHub | **My skills** — enable, view, remove |
| <img src="docs/screenshots/05-plugins.png" alt="Plugins" /> | <img src="docs/screenshots/07-connectors-catalog.png" alt="Connectors" /> |
| **Plugins** — official Anthropic marketplace | **Connectors** — one-click MCP |
| <img src="docs/screenshots/08-models.png" alt="Models" /> | <img src="docs/screenshots/11-shortcuts.png" alt="Shortcuts" /> |
| **Local AI** — 6-step connection test | **Keyboard shortcuts** |
| <img src="docs/screenshots/06-connectors.png" alt="My connectors" /> | <img src="docs/screenshots/10-settings-ru.png" alt="Settings in Russian" /> |
| **My connectors** — status and tools | **Three languages** — Русский shown |

## Download & install

1. Download **`Sakina-AI-Desktop-Setup-<version>.exe`** from the [latest release](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest).
2. Run it and follow the wizard (install for you only or for all users, choose the folder).
3. Windows SmartScreen may warn because the installer is not code-signed yet: click **More info → Run anyway**.

**Requirements:** Windows 10 or 11 (x64), 4 GB RAM (8 GB+ recommended), ~500 MB of disk space. Node.js is needed only for local MCP connectors (npx).

### Updating

Sakina checks GitHub Releases at start and every 4 hours (can be turned off in *Settings → Updates*). When a new version appears, a card slides open in the sidebar: **GitHub** opens the release notes, **Update** downloads it with a progress bar, verifies its SHA-512 and offers **Restart and update**. Installing a newer installer manually works too — it shows **Update 1.x → 1.y** instead of *Install* and keeps your chats, projects, settings and keys.

## Your own model on another computer

Run the model on the GPU machine, use it from your laptop:

```bash
# On the GPU PC (Ollama example): listen on the local network
setx OLLAMA_HOST 0.0.0.0
ollama serve
```

In Sakina: **Models → Local AI → Add local server**, pick the server type (Ollama, Open WebUI, vLLM, SGLang, LM Studio, Kimi K2…), enter the IP and press **Test**. If the address belongs to a different server (for example an Open WebUI page instead of its API), the test detects it and offers **Apply**.

## Privacy

- No telemetry, no accounts, no ads.
- Data lives in `%APPDATA%\sakina-ai-desktop` on your computer.
- Requests go only to the providers and connectors you configure; update checks contact GitHub.
- API keys and connector tokens are encrypted with Windows DPAPI and never written to logs or exports.

## FAQ

**Is it free?** Yes — Sakina AI Desktop is free to use for personal and commercial work under the [EULA](LICENSE.md). AI providers bill you according to their own prices.

**Do I need an internet connection?** Not with local models. Cloud providers, the skills/plugins catalogs and update checks need internet.

**Can I use Claude Code skills and plugins?** Yes: Skills use the same `SKILL.md` format, and plugins in Claude Code format contribute their skills, slash commands and MCP servers. Subagents and hooks are listed but not executed.

## License

Sakina AI Desktop is proprietary freeware — see the [End User License Agreement](LICENSE.md). Open-source components are used under their own licenses (included with the app).

## Author

Developed by **Imomzoda Mehriddin** · [github.com/imomzoda-dev](https://github.com/imomzoda-dev)

Found a bug or have an idea? [Open an issue](https://github.com/imomzoda-dev/SakinaAiDesktop/issues).
