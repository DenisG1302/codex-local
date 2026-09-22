<div align="center">
  <img src="assets/logo.png" width="80" height="80" alt="Codex Local">
  <h1>Codex Local</h1>
  <p>Your Codex — on your PC, in a browser and on your phone.</p>
  <p><strong>Windows x64 · local panel · web access and PWA</strong></p>
  <p><a href="https://github.com/DenisG1302/codex-local/releases/latest"><strong>Download installer</strong></a> · <a href="https://github.com/DenisG1302/codex-local/releases">Release notes</a> · <a href="README.md">Русский</a></p>
</div>

---

Codex Local is an independent Windows app that connects to your installed Codex through App Server. Organize chats by project, run several tasks at once and access your workspace in the desktop app, a local browser or another device.

This repository contains **installers and documentation**. Application source code is maintained separately and is not published here. This app is not an official OpenAI product.

## Features

| Feature | Purpose |
| --- | --- |
| Windows app and local web | Open the same panel in a dedicated window or a browser on your PC |
| Local network access | Work from a phone, tablet or another computer on your network |
| Your own HTTPS domain | Access the panel remotely through a domain and reverse proxy you configure |
| Mobile PWA | Add the panel to your home screen, use the responsive layout and receive push notifications |
| Up to five chat panes | Choose a layout and follow several tasks at once |
| Focus layout | Read one large chat and switch through cards for active tasks and unread replies; the card list is not limited to five |
| Smart pane selection | Fill expanded layouts with running and waiting chats in project order, preserving your selected active chat |
| Projects and pins | Group tasks, distinguish projects by color, pin chats and drag to reorder |
| Search and quick navigation | Find chats and projects by name; open search and actions with Ctrl+K or a custom shortcut |
| Message bookmarks | Save important replies and return to their place in the conversation |
| Model and reasoning controls | Choose an available model, reasoning effort and speed mode; remember your selection per chat |
| Status, subagents and usage | See compact task status and inspect active subagent work |
| Work history controls | Hide details of completed requests while ongoing work, questions and answers remain visible |
| Questions and approvals | Answer in the panel, attach images and confirm supported tool requests |
| Persistent drafts | Keep unfinished text and uploaded attachments separately for each chat after restarting |
| Message queue | Prepare, edit and reorder upcoming messages |
| Comfortable writing and follow-ups | Expand the composer without jumping the conversation; group follow-ups with the original request after completion |
| Code viewer | Open files inside the panel with language labels, highlighting, search and line navigation |
| File path and actions | Copy the full path; in the Windows app, open the default application, use the native Open With chooser, or reveal the file in its folder |
| Change navigation | Start at the first change and jump between marked sections, including changes deep inside large files |
| Final file summary | See every file touched during a request, labeled Created, Modified or Deleted, in batches of five |
| HTML previews | Open interactive mockups with local CSS and JavaScript next to your chat |
| Limits and usage | See remaining allowance, renewal time and approximate request usage |
| Available resets | Review reset credits reported by Codex and redeem them with separate confirmation when supported by your account |
| Reset announcements | Read localized Codex Resets statuses and possible reset times in your device's time zone |
| Live theme previews | Choose light, dark and high-contrast palettes, or set your own background and accent colors |
| Relevant notifications | Receive completions, questions and approval requests; visible chats in the foreground do not generate unnecessary notifications |
| Tray operation | Close the window while tasks and web access continue; optionally start with Windows |
| Responsive long conversations | Use cached history, partial streaming updates and background highlighting for large files |
| One-button updates | Check, download and install signed releases while ongoing tasks continue running |

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
