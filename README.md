<div align="center">

<img src="docs/logo.png" width="96" alt="Sakina AI Desktop logo" />

# Sakina AI Desktop

**Your AI workspace on Windows. Chat with any cloud or local model, let an agent work in your code and terminal, and create documents, slides, designs and dashboards — with your data staying on your computer.**

[![Latest release](https://img.shields.io/github/v/release/imomzoda-dev/SakinaAiDesktop?label=release&color=D97757)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/total?color=D97757)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-0078d4)
![Languages](https://img.shields.io/badge/UI-English%20%7C%20Русский%20%7C%20Тоҷикӣ-6b7280)
[![License](https://img.shields.io/badge/license-EULA%20(freeware)-6b7280)](LICENSE.md)

[**⬇ Download Sakina 1.3.6 for Windows**](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest) · [What's new](#-whats-new-in-136) · [Changelog](CHANGELOG.md) · [Русский](README.ru.md)

<img src="docs/screenshots/chat.png" alt="Sakina AI Desktop — chat" width="900" />

</div>

---

## ✨ What's new in 1.3.6

- **Profile photo.** Click your photo in *Settings → Account & Profile* or drop a picture on it, then crop it in a round frame (drag, zoom with the slider, the mouse wheel or the keyboard). It is saved as a 512×512 JPEG without location or camera data, stored in your account and shown on every computer. Google accounts can switch back to their Google photo.
- **A redesigned Account & Profile page** with a cover, a large photo, your sign-in methods and clear sections — profile, personal touch, sign-in & security and a separate danger zone.
- **Password strength meter.** Instead of a checklist, a four-step meter fills and changes colour as you type and gives one useful tip.
- **Continue with Google.** Sign in or create your account with Google in one click. Google's page opens in your own browser — your Google password never passes through Sakina — and Sakina comes back to the front already signed in. Your name and photo come from Google; an existing e-mail account with the same address simply gets a second way to sign in, and you can add a password later in *Settings → Account*.
- **Design, rebuilt as a gallery.** Everything you create lives in one place, like Claude's Artifacts: cards with a live preview, the time of the last edit, favorites, search, filters by type and sorting. Hover a card to open it full screen, present a deck, duplicate or delete it.
- **New: Documents.** Reports, proposals, articles, guides, plans and resumes, laid out like a printed page with a title block, numbered sections, tables, callouts and charts. Export to PDF (A4), PNG or HTML.
- **New: Dashboards.** KPI tiles, interactive charts, filters that really work and a sortable table, built from sample data for your field, in light and dark themes.
- **Full screen and presenting.** Any document, design or dashboard opens full screen (`F`) with desktop, tablet and phone frames. Decks present from the current slide (`F5`): arrows, a click or Space for the next slide, a progress line, and an overview of all slides (`G`). The controls hide while you read; `Esc` brings you back exactly where you were.
- **Smoother background work.** “Minimize to background” now flies the window into its capsule at the top right and grows it back when you open it again.
- **Image export.** Save a full-length PNG of any design, document or dashboard.
- **A new About page** with the live GitHub repository (stars, forks, downloads, latest release), what you have done in Sakina on this computer, update status and one-click system details for bug reports.


<p align="center">
  <img src="docs/screenshots/account.png" alt="Account & Profile with a profile photo" width="49%" />
  <img src="docs/screenshots/password-strength.png" alt="Password strength meter" width="49%" />
</p>
<p align="center">
  <img src="docs/screenshots/google-sign-in.png" alt="Continue with Google" width="70%" />
</p>

<p align="center">
  <img src="docs/screenshots/design-gallery.png" alt="Design gallery with live previews" width="49%" />
  <img src="docs/screenshots/design-document.png" alt="A document in the Design editor" width="49%" />
</p>
<p align="center">
  <img src="docs/screenshots/design-dashboard.png" alt="A dashboard made by AI" width="49%" />
  <img src="docs/screenshots/design-fullscreen.png" alt="Full screen view" width="49%" />
</p>
<p align="center">
  <img src="docs/screenshots/design-present.png" alt="Presenting a deck" width="49%" />
  <img src="docs/screenshots/design-overview.png" alt="Overview of all slides" width="49%" />
</p>

## Why Sakina

- **Any model, one app.** OpenAI, Anthropic Claude, Google Gemini, OpenRouter, Groq, DeepSeek, Mistral, Moonshot Kimi and any OpenAI-compatible API — **plus your own models**: Ollama, Open WebUI, vLLM, SGLang, llama.cpp, LM Studio, Kimi K2 self-hosted and more local or LAN servers.
- **Private by design.** No telemetry. Chats, projects, files, designs and API keys stay on your PC; keys are encrypted with Windows DPAPI. Route sensitive projects to local models only.
- **An agent that really works.** It reads and edits files, runs commands in your terminal, uses Git, asks you questions and runs subagents — every risky action waits for your approval, and every change can be rewound.
- **Create, not just chat.** Documents, slide decks, interfaces, dashboards and design systems, refined by text, versioned and exported to PDF, PowerPoint, PNG or HTML.
- **Claude-style extensibility.** Skills (`SKILL.md`), Connectors (MCP), Plugins and Agents in the Claude Code format — install popular ones from GitHub in one click.
- **Updates itself.** New versions are found on GitHub Releases, downloaded with progress, verified (SHA-512) and installed with one click — your data stays.

## A quick tour

### Chat

Streaming answers with Markdown, tables, code, Mermaid and HTML previews, reasoning blocks, attachments (PDF, Office, images), voice input, branching edits and search. Sakina greets you by name and remembers your drafts.

<p align="center">
  <img src="docs/screenshots/welcome.png" alt="Welcome screen" width="49%" />
  <img src="docs/screenshots/chat.png" alt="A chat with a formatted answer" width="49%" />
</p>

### Design

Six kinds of work: **Document**, **Slides**, **Design**, **Dashboard**, **Design in codebase** (follows your project's tokens and components) and **Design system**. Generation runs in the background — minimize it and keep working; a capsule shows the progress and opens the result when it is ready.

<p align="center">
  <img src="docs/screenshots/design-progress.png" alt="Generation progress" width="49%" />
  <img src="docs/screenshots/design-background.png" alt="Generation continues in the background" width="49%" />
</p>

### Code workspace

Explorer, Monaco editor with IntelliSense, Ctrl+P quick open, project tasks, background processes, a terminal (PowerShell, CMD, Git Bash), Git, and an AI panel you can collapse to a slim rail (`Ctrl+Alt+B`). The agent works with checkpoints, hooks, subagents and questions.

<img src="docs/screenshots/code-workspace.png" alt="Code workspace with the AI panel" width="100%" />

### AI Workspace

A personal dashboard you change by talking to it: calendar, tasks, system and model monitors, charts, stats and your own sandboxed widgets — with undo, snapshots and export.

<img src="docs/screenshots/ai-workspace.png" alt="AI Workspace" width="100%" />

### Agents and Training

Create specialised agents (or draft one with AI), browse a catalog of open-source agents, and train your own model: build an Ollama model from a course or your data, compare it with the base model, or get a LoRA kit sized for your GPU.

<p align="center">
  <img src="docs/screenshots/agents.png" alt="Agents" width="49%" />
  <img src="docs/screenshots/training.png" alt="Training" width="49%" />
</p>

### Skills, Connectors and Plugins

A catalog of 232 popular skills in 13 categories, 58 verified MCP connectors (GitHub, Context7, Notion, Playwright, Supabase…) and the official Anthropic plugin marketplace — installed in one click, tokens stored encrypted.

<p align="center">
  <img src="docs/screenshots/skills.png" alt="Skills catalog" width="49%" />
  <img src="docs/screenshots/connectors.png" alt="Connectors" width="49%" />
</p>

### Models, account and About

Connect cloud providers and your own servers on the local network with a 6-step connection test. Your Sakina account keeps your name and setup across computers; the About page shows the version, the GitHub repository and your activity.

<p align="center">
  <img src="docs/screenshots/models.png" alt="Local and LAN models" width="49%" />
  <img src="docs/screenshots/about.png" alt="About page" width="49%" />
</p>

## All features

| | |
|---|---|
| 💬 **Chat** | Streaming, Markdown, tables, code highlighting, Mermaid, HTML/SVG preview, reasoning blocks, attachments incl. PDF and Office, voice input, branching edits, search, export, response styles, slash commands |
| 🎨 **Design** | Documents, slides, designs, dashboards, designs in your codebase and design systems; gallery with live previews, versions, device preview, full screen and presenting with slide overview, background generation; PDF / PowerPoint / PNG / HTML export |
| 🛠️ **Code workspace & agent** | Explorer, Monaco editor, Ctrl+P, tasks, background processes, status bar, terminal, Git, collapsible AI panel, subagents, questions from the agent, hooks, checkpoints and rewind, approvals for risky actions |
| 🪄 **AI Workspace** | Widgets and dashboards created and changed from the chat, 12 built-in widgets, sandboxed custom widgets, drag and drop, undo/redo, snapshots, export/import |
| 🤖 **Agents** | Your own agents in the Claude Code subagent format, drafted with AI, plus a catalog of open-source agents |
| 🎓 **Training** | Ollama model builds from courses or your data, side-by-side tests against the base model, GPU-aware LoRA kits |
| 🧠 **Models & routing** | Cloud and local providers, multi-key rotation, health of local servers, automatic default model, smart / privacy-first / local-only routing |
| 🖥️ **Local & LAN AI** | 28 server types with a 6-step connection test; detects Open WebUI / Ollama / OpenAI-compatible servers and fixes the address in one click |
| ✨ **Skills, Connectors, Plugins** | 232 skills, 58 MCP connectors, the official Anthropic marketplace and any GitHub marketplace in Claude Code format |
| 📄 **Any file** | Word, Excel, PowerPoint, PDF, images, audio and video open inside the app |
| 👤 **Account** | Continue with Google or sign in with e-mail (confirmation, password reset, strength meter), profile photo with cropping, a one-time setup, profile and name on every computer, full account deletion |
| 🧭 **Comfort** | Global hotkey `Ctrl+Shift+Space`, tray icon, command palette `Ctrl+K`, shortcuts `Ctrl+/`, light and dark themes, English, Russian and Tajik interface |
| 🔒 **Safety** | Path guard, command risk analysis, permission rules, audit log, encrypted secrets, backups with SHA-256 verification, database copy before every schema upgrade |

## Download & install

1. Download **`Sakina-AI-Desktop-Setup-1.3.6.exe`** from the [latest release](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/latest).
2. Run it and follow the wizard (install for you only or for all users, choose the folder).
3. Windows SmartScreen may warn because the installer is not code-signed yet: click **More info → Run anyway**.
4. Continue with Google or create a Sakina account with your e-mail, answer the short setup once — and you are ready.

**Requirements:** Windows 10 or 11 (x64), 4 GB RAM (8 GB+ recommended), about 500 MB of disk space. Node.js is needed only for local MCP connectors (npx).

### Updating

Sakina checks GitHub Releases at start and every 4 hours (you can turn it off in *Settings → Updates*). When a new version appears, a card slides open in the sidebar: **Update** downloads it with a progress bar, verifies its SHA-512 and offers **Restart and update**. Installing a newer installer manually works too — your chats, projects, designs, settings and keys are kept.

## Your own model on another computer

Run the model on the GPU machine and use it from your laptop:

```bash
# On the GPU PC (Ollama example): listen on the local network
setx OLLAMA_HOST 0.0.0.0
ollama serve
```

In Sakina: **Models → Local AI → Add local server**, pick the server type (Ollama, Open WebUI, vLLM, SGLang, LM Studio, Kimi K2…), enter the IP and press **Test**. If the address belongs to a different server (for example an Open WebUI page instead of its API), the test detects it and offers **Apply**.

## Privacy

- No telemetry and no ads.
- Chats, files, projects, designs and settings live in `%APPDATA%\sakina-ai-desktop` on your computer. Chat history is never uploaded.
- Your Sakina account stores only your e-mail, name, photo (with Google) and setup answers; with Google sign-in Sakina never sees your Google password; you can delete the account and all of it at any time in *Settings → Account*.
- Requests go only to the AI providers and connectors you configure; update checks contact GitHub.
- API keys, connector tokens and the sign-in session are encrypted with Windows DPAPI and never written to logs or exports.

## FAQ

**Is it free?** Yes — Sakina AI Desktop is free for personal and commercial use under the [EULA](LICENSE.md). AI providers bill you according to their own prices.

**Do I need an internet connection?** Not for local models. Signing in, cloud providers, the catalogs and update checks need internet.

**Which model should I use for Design?** A strong model with a large output limit gives the best documents, decks and dashboards. Raise *Max output tokens* of the model in *Models* if a long design stops early.

**Can the AI break the app by changing the interface?** No. The model only sends declarative operations that are validated before anything changes; generated code runs in an isolated sandbox; every change can be undone.

**Can I use Claude Code skills, plugins and agents?** Yes: Skills use the same `SKILL.md` format, plugins contribute their skills, slash commands and MCP servers, agents use the subagent format, and hooks run with the same exit-code rules.

## Downloads by version

| Version | Downloads |
|---|---|
| [v1.3.6](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.6) | [![v1.3.6](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/v1.3.6/total?label=downloads&color=D97757&style=flat-square)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.6) |
| [v1.3.5](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.5) | [![v1.3.5](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/v1.3.5/total?label=downloads&color=D97757&style=flat-square)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.5) |
| [v1.3.4](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.4) | [![v1.3.4](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/v1.3.4/total?label=downloads&color=D97757&style=flat-square)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.4) |
| [v1.3.3](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.3) | [![v1.3.3](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/v1.3.3/total?label=downloads&color=D97757&style=flat-square)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases/tag/v1.3.3) |
| **All versions** | [![Total](https://img.shields.io/github/downloads/imomzoda-dev/SakinaAiDesktop/total?label=total&color=D97757&style=flat-square)](https://github.com/imomzoda-dev/SakinaAiDesktop/releases) |

Counters come live from GitHub; the app shows the same numbers in *Settings → About* and *Settings → Updates*.

## License

Sakina AI Desktop is proprietary freeware — see the [End User License Agreement](LICENSE.md). Open-source components are used under their own licenses (included with the app).

## Author

Developed by **Imomzoda Mehriddin** · [github.com/imomzoda-dev](https://github.com/imomzoda-dev)

Found a bug or have an idea? [Open an issue](https://github.com/imomzoda-dev/SakinaAiDesktop/issues).
