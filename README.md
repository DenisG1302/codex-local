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

![Codex Local desktop workspace with projects, a launch checklist and usage limits](assets/screenshots/en/workspace-light.png)

<p align="center"><sub>Codex Local 0.8.33 · Actual interface with demo projects and conversations.</sub></p>

## Features

The interface is available in English and Russian. Choose your language in **Settings → Appearance**.

| Feature | What it adds |
| --- | --- |
| Limits at a glance | Remaining allowance, renewal times and estimated request usage in one place |
| Resets and forecasts | Available resets with confirmation, plus announcements of possible resets from Codex Resets |
| Multiple chats at once | Up to five side-by-side panes, or Focus: one large chat with cards for active and unread tasks |
| Always-on-top window | Full latest progress and actions above your other apps, with pinning and active and unread chat switching |
| Replies to messages | Reply to a message or selected passage with context above the composer; replies go first in a busy chat’s queue |
| Forwarding between chats | Prepare a message with files and photos in another chat, add a comment and send when ready |
| Quick commands | Send a saved reply with one click; add your own choices and remove ones you do not need |
| Rules with Codex | Edit global instructions or a project’s AGENTS.md; review the assistant’s proposed changes before applying them |
| Model and fast mode | Choose a model and reasoning level; control the speed of the current task separately from the next message |
| Message queue | Edit text, attachments and model settings for each waiting message, and rearrange their order |
| Your own web access | Use the panel in a local browser, over your network or through your own HTTPS domain |
| Phone and PWA | Access chats from your phone and add the panel to your home screen |
| Notification preferences | Choose events, Windows and Web Push delivery, notification sounds, and message previews |
| Themes that fit you | Ten light and ten dark palettes, high contrast, and custom background and accent colors with live previews |

## Always-on-top window

Open the window from the chat header. On Windows it stays above other apps and can open automatically when Codex Local is minimized or in the background. Pin it to prevent accidental dragging. The arrow switches between active and unread chats; viewing the window does not mark answers as read.

The window shows the full latest progress message and current actions. When a task finishes, it displays **Work finished**; **Open chat** takes you to the full answer.

In **Settings → Appearance**, choose a text style, window style, the theme color or your own color. Long text can scroll manually, scroll automatically from top to bottom in a loop, or grow the window within the screen. Set the default size, position, opacity and automatic opening there too. Disabling the feature hides the chat button and detailed settings. Supported browsers offer manual opening with Picture-in-Picture.

| Progress window | Compact settings |
| --- | --- |
| [![Always-on-top window with latest progress, actions, pinning and chat switching](assets/screenshots/en/overlay.png)](assets/screenshots/en/overlay.png) | [![Long-text modes, text and window styles, default size and automatic opening](assets/screenshots/en/overlay-settings.png)](assets/screenshots/en/overlay-settings.png) |

## Rules with the Codex assistant

Open **Settings → Instructions** to edit global rules or the selected project’s **AGENTS.md**. If the project has no rules file yet, create it from the same screen.

The assistant can add, remove or edit a rule, organize the existing text, or follow your own **Custom** request. **Organize** also works without a description. Choose the assistant’s model and reasoning level separately from your chat settings, then review the proposed full text or line changes. You can edit the proposal, apply it with **Apply**, or decline it. Changes apply to new chats; existing chats may keep their previous instructions.

## Model, fast mode and message queue

The control beside the composer combines model, reasoning level and fast mode. The speed control beside the running status changes the current task separately, after confirmation. Fast mode is available for supported models and uses more of your allowance.

Messages sent while a task is running wait in a queue. Rearrange them, edit their text and attachments, or choose a different model, reasoning level and speed for each one. **Steer** sends a waiting message into the current task using that task’s settings. The queue survives a restart and continues to work without an open window.

## Replies, forwarding and quick commands

Open a message’s **⋯ menu** and choose **Write a reply**. The selected message appears above the composer; write your reply without copying the full original text. To reply to a specific passage, select it and press **Reply**. Your existing draft stays in place.

On phones, **Reply** appears on the right, aligned with the message field's first line and separate from the native selection menu. Tapping it scrolls the chat to the bottom and keeps the reply field and Send button above the keyboard. Tap outside the field to dismiss the keyboard and keep your draft. Cancelling a reply dismisses the keyboard only when the field is empty; if text is already written, editing stays active.

**Forward** prepares the selected message with its files and photos in another chat. Choose a project, then a new chat or one of the five most recent chats; load five more when needed. A card appears above the destination composer: add a comment, keep it as a draft or cancel it. The message is sent only when you press **Send**. After sending, you can also notify the source chat that the original message was meant for another chat.

Quick commands are saved replies in the same message menu. Use **Manage quick replies** to add your own phrases or remove any choice, including **This was not meant for you**. While a chat is busy, replies to messages or selected passages, including quick replies, go to the front of its queue and wait for the current task to finish.

## Screenshots

### Review rule changes before applying them

Choose the rules to edit, describe the change and compare the assistant’s proposal with the current text. Apply it when you are ready.

![Project rules and the Codex assistant, with a proposed rule highlighted and Apply and Decline controls](assets/screenshots/en/instructions.png)

### Plan the next messages

Each queued message has its own model, reasoning level and speed. Edit a waiting message while the current task continues.

![Message queue with different model settings and an open model, reasoning and fast-mode picker](assets/screenshots/en/queue-model.png)

### Keep several tasks in view

Focus mode gives the current conversation more room while keeping running tasks and unread results alongside it.

![Focus mode in the dark Polar theme with one large conversation and four task cards](assets/screenshots/en/focus-dark.png)

### Open files beside the conversation

Read code with syntax highlighting and line numbers, search within a file, and stay in the same chat.

![TypeScript component open in the file viewer beside its conversation](assets/screenshots/en/code-preview.png)

### Make the workspace yours

Pick separate light and dark palettes, then choose the events, delivery channels and message previews you want.

| Appearance and language | Notification preferences |
| --- | --- |
| [![Appearance settings with English selected and light and dark color palettes](assets/screenshots/en/appearance.png)](assets/screenshots/en/appearance.png) | [![Notification settings with event filters, PC and Web Push channels, and message preview controls](assets/screenshots/en/notifications.png)](assets/screenshots/en/notifications.png) |

### Take your chats with you

The mobile layout keeps conversations, projects and usage limits within reach. Your Windows PC continues to run the tasks.

<p align="center">
  <a href="assets/screenshots/en/mobile-chat.png"><img src="assets/screenshots/en/mobile-chat.png" width="340" alt="Mobile conversation with a completed navigation review and the message composer"></a>
  <a href="assets/screenshots/en/mobile-projects.png"><img src="assets/screenshots/en/mobile-projects.png" width="340" alt="Mobile project list with active tasks, usage limits and settings"></a>
</p>

Select a passage and press **Reply** in the composer. The button sits on the right, aligned with the message field's first line and separate from the native actions for selected text.

<p align="center"><a href="assets/screenshots/en/mobile-reply.png"><img src="assets/screenshots/en/mobile-reply.png" width="340" alt="Selected passage in a mobile chat with Reply on the right, aligned with the message field's first line"></a></p>

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
