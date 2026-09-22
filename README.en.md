<div align="center">
  <img src="assets/logo.png" width="80" height="80" alt="Codex Local">
  <h1>Codex Local</h1>
  <p>Your projects. Multiple chats. One workspace.</p>
  <p><strong>Windows x64 · local panel · web access and PWA</strong></p>
  <p><a href="https://github.com/DenisG1302/codex-local/releases/latest"><strong>Download installer</strong></a> · <a href="https://github.com/DenisG1302/codex-local/releases">Release notes</a> · <a href="README.md">Русский</a></p>
</div>

---

Codex Local is an independent Windows app that connects to your installed Codex through App Server. Organize chats by project, follow several tasks, and return to important answers without losing context.

This repository contains **installers and documentation**. Application source code is maintained separately and is not published here. This app is not an official OpenAI product.

## Features

| Feature | Purpose |
| --- | --- |
| Multiple chats and Focus | One large chat alongside cards for active tasks and unread replies |
| Projects, search and bookmarks | Find conversations and save important messages |
| Work history | Follow the current task and control visibility of completed work |
| Files and changes | Read highlighted code, jump between changes and preview HTML |
| Themes | Light, dark and custom colors with live preview |
| Drafts and queue | Keep unfinished input and prepare follow-up messages |
| Notifications and PWA | Receive questions and results; access the panel from other devices |
| Verified updates | Install signed releases while ongoing tasks continue running |

## Installation

1. Install **Codex for Windows** and sign in to your own account. You need access to Codex; this panel does not include a subscription or increase usage limits.
2. Download **`Codex-Local-Setup-…exe`** from the [latest release](https://github.com/DenisG1302/codex-local/releases/latest).
3. Run the installer and open Codex Local. Create a local panel account on first launch.

Requires Windows x64 and Microsoft Edge WebView2 Runtime. Node.js is included. The application interface is currently in Russian; documentation and new release notes are available in Russian and English.

No GitHub account, private repository access or development tools are required to download the installer. The **Source code** archives automatically added by GitHub contain only this repository's documentation. Choose the EXE to install the app.

## Updates

Open **Settings → Updates** (**Настройки → Обновления**). The page shows your installed version. **Check and update** (**Проверить и обновить**) downloads, verifies and installs a newer release automatically. The app also notifies you about available updates at startup. Ongoing tasks run in a separate process and continue while the panel is updated.

An update must have a valid release signature and a matching EXE checksum. This is the application's update verification, not a Windows publisher certificate. Windows may display an unknown-publisher warning. Download your first installation only from this repository.

## Data and access

The installer contains no other user's accounts, conversations, project files or connection settings. Panel data is created on your PC under `%LOCALAPPDATA%\CodexLocal`; Codex manages its own authentication. The panel contacts GitHub for updates and Codex Resets for public reset announcements. Model requests are processed by the services your Codex connects to.

Web access is protected by the panel's local account. To connect a phone, open **Settings → Connection**. PWA push notifications require configured HTTPS access. Keep your panel password and authentication files private.

## Feedback

[Open an issue](https://github.com/DenisG1302/codex-local/issues/new) with the app version, expected behavior and reproduction steps. Remove personal information from screenshots. Do not attach tokens, session directories or complete logs containing private conversations.

Third-party component license notices are included with the installation. Public availability of the installer does not make the application source code public.
