<div align="center">

<img src="logo.svg" width="96" height="96" alt="Flightdeck logo" />

# Flightdeck

**Run & control all your local dev servers, ports and services in one place.**

[![Latest release](https://img.shields.io/github/v/release/coderrumaro/flightdeck-releases?label=Latest&style=for-the-badge)](https://github.com/coderrumaro/flightdeck-releases/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-x64-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/coderrumaro/flightdeck-releases/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-Universal-000000?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/coderrumaro/flightdeck-releases/releases/latest)

[Download latest release](https://github.com/coderrumaro/flightdeck-releases/releases/latest) · [All releases](https://github.com/coderrumaro/flightdeck-releases/releases)

</div>

---

Flightdeck is a desktop app for developers who juggle multiple repos and dev servers. Point it at your projects folder, and every `package.json` script becomes a one-click **Start** / **Stop** with its own live terminal — like VS Code, but for your whole machine at once.

See **everything** listening on a port (Flightdeck, VS Code, Cursor, Docker, terminals) and kill anything by port or PID when you need a clean slate.

> This repository publishes **installers only**. Application source code is not published here.

## Download

Go to **[Releases](https://github.com/coderrumaro/flightdeck-releases/releases/latest)** and pick the file for your OS:

| Platform | File | Notes |
| -------- | ---- | ----- |
| **Windows** | `Flightdeck_*_x64-setup.exe` | Recommended — NSIS installer |
| **Windows** | `Flightdeck_*_x64_en-US.msi` | MSI installer (IT / enterprise) |
| **macOS** | `Flightdeck_*_universal.dmg` | Apple Silicon + Intel in one build |

### First launch (unsigned builds)

Installers are **unsigned** today. Your OS will ask for a one-time confirmation — this is normal, not a sign the file was tampered with.

- **macOS:** Right-click the app → **Open** → **Open** again in the dialog.
- **Windows:** If SmartScreen appears → **More info** → **Run anyway**.

## What you get

- **Repo scanner** — finds every `package.json` in a folder (monorepos included), detects npm / pnpm / yarn / bun, shows git branch and dirty state.
- **One-click scripts** — Start turns into Stop with uptime, health dot, CPU/RAM/PID, bound `localhost` URL, restart, pin, and auto-restart on crash.
- **Live terminals** — real PTY per script (ConPTY on Windows), stdin support, log filter (All / Warn / Err), plus a per-repo **Shell** tab.
- **Running view** — all TCP listeners and Docker containers, grouped by type, with owner badges and kill-by-port/PID.
- **Dashboard** — running servers, ports, CPU/RAM tiles, sparkline, quick-launch stacks, needs-attention list.
- **Command palette** (`Ctrl+K` / `⌘K`) — start/stop any command, launch a stack, jump to a repo, kill a port.
- **Stacks** — save a group of commands and start them together.
- **Pinned bar** — pin favourites with `Ctrl+Alt+1`–`9` (Windows) or `⌥⌘1`–`9` (macOS).
- **Light / dark / system** theme, keyboard navigation, tray minimize on close.

## Keyboard shortcuts

| Shortcut | Action |
| -------- | ------ |
| `Ctrl+K` / `⌘K` | Command palette |
| `Ctrl+,` / `⌘,` | Settings |
| `Ctrl+Alt+1`–`9` / `⌥⌘1`–`9` | Toggle pinned commands |

## System requirements

- **Windows 10/11** (64-bit) with WebView2 (preinstalled on modern Windows)
- **macOS 11+** (Apple Silicon or Intel)

## Privacy & data

Flightdeck runs **locally on your machine**. Repo paths, scripts, and preferences are stored in your OS app config folder — not sent to a cloud service by this app.

| OS | Config location |
| -- | --------------- |
| Windows | `%APPDATA%\com.coderrumaro.flightdeck\` |
| macOS | `~/Library/Application Support/com.coderrumaro.flightdeck/` |

---
