<div align="center">
  <img src="assets/logo.png" width="80" height="80" alt="Codex Local">
  <h1>Codex Local</h1>
  <p>Your Codex — on your PC, in a browser and on your phone.</p>
  <p><strong>Windows x64 · local panel · web access and PWA</strong></p>
  <p><a href="https://github.com/DenisG1302/codex-local/releases/latest"><strong>Download installer</strong></a> · <a href="https://github.com/DenisG1302/codex-local/releases">Release notes</a> · <a href="README.ru.md">Русский</a></p>
</div>

---

Codex Local is an independent Windows app that connects to your installed Codex through App Server. Organize chats by project, run several tasks at once and access your workspace in the desktop app, a local browser or another device.

This repository contains **installers and documentation**. Application source code is maintained separately and is not published here. This app is not an official OpenAI product.

![Codex Local desktop workspace with projects, a launch checklist and usage limits](assets/screenshots/workspace-light.png)

<p align="center"><sub>Codex Local 0.8.6 · Actual interface with demo projects and conversations.</sub></p>

## Features

The interface is available in English and Russian. Choose your language in **Settings → Appearance**.

| Feature | What it adds |
| --- | --- |
| Limits at a glance | Remaining allowance, renewal times and estimated request usage in one place |
| Resets and forecasts | Available resets with confirmation, plus announcements of possible resets from Codex Resets |
| Multiple chats at once | Up to five side-by-side panes, or Focus: one large chat with cards for active and unread tasks |
| Your own web access | Use the panel in a local browser, over your network or through your own HTTPS domain |
| Phone and PWA | Access chats from your phone and add the panel to your home screen |
| Notification preferences | Choose events, Windows and Web Push delivery, notification sounds, and message previews |
| Themes that fit you | Ten light and ten dark palettes, high contrast, and custom background and accent colors with live previews |

## Screenshots

### Keep several tasks in view

Focus mode gives the current conversation more room while keeping running tasks and unread results alongside it.

![Focus mode in the dark Polar theme with one large conversation and four task cards](assets/screenshots/focus-dark.png)

### Open files beside the conversation

Read code with syntax highlighting and line numbers, search within a file, and stay in the same chat.

![TypeScript component open in the file viewer beside its conversation](assets/screenshots/code-preview.png)

### Make the workspace yours

Pick separate light and dark palettes, then choose the events, delivery channels and message previews you want.

| Appearance and language | Notification preferences |
| --- | --- |
| [![Appearance settings with English selected and light and dark color palettes](assets/screenshots/appearance.png)](assets/screenshots/appearance.png) | [![Notification settings with event filters, PC and Web Push channels, and message preview controls](assets/screenshots/notifications.png)](assets/screenshots/notifications.png) |

### Take your chats with you

The mobile layout keeps conversations, projects and usage limits within reach. Your Windows PC continues to run the tasks.

<p align="center">
  <a href="assets/screenshots/mobile-chat.png"><img src="assets/screenshots/mobile-chat.png" width="340" alt="Mobile conversation with a completed navigation review and the message composer"></a>
  <a href="assets/screenshots/mobile-projects.png"><img src="assets/screenshots/mobile-projects.png" width="340" alt="Mobile project list with active tasks, usage limits and settings"></a>
</p>

## Ways to connect

| Option | How to open it |
| --- | --- |
| On this PC | Use the Codex Local app or open `http://127.0.0.1:4317` in a browser; the port is configurable |
| On your network | Open **Settings → Connection → Local network**, copy the PC address and open it on another device |
| Over the internet | Configure an HTTPS domain and reverse proxy to the panel, then enter the address in **Settings → Connection → Domain** |
| As a phone app | Open the HTTPS address in a browser, add the panel to your home screen and enable notifications in settings |

All devices connect to the same panel on your Windows PC: project files and task execution remain there. Keep the computer awake and Codex Local running, including in the tray. Set up the domain, certificate and external routing separately; the panel does not provision them automatically. Regular web access over a local IP works without a domain; PWA installation and push on other devices require HTTPS and browser support.

Usage estimates rely on the counters Codex provides and can include other tasks running in parallel. Codex Resets predictions come from a third-party announcement service and do not guarantee a reset. Requests that specifically require confirmation in Codex open in its desktop app.

## Data and access

The installer contains no other user's accounts, conversations, project files or connection settings. Panel data is created on your PC under `%LOCALAPPDATA%\CodexLocal`; Codex manages its own authentication. The panel contacts GitHub for updates and Codex Resets for public reset announcements. Model requests are processed by the services your Codex connects to.

Web access is protected by the panel's local account. To connect a phone, open **Settings → Connection**. PWA push notifications require configured HTTPS access. Keep your panel password and authentication files private.

## Feedback

[Open an issue](https://github.com/DenisG1302/codex-local/issues/new) with the app version, expected behavior and reproduction steps. Remove personal information from screenshots. Do not attach tokens, session directories or complete logs containing private conversations.

Third-party component license notices are included with the installation. Public availability of the installer does not make the application source code public.
