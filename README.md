# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

MyCodex turns Codex + Hermes into a desktop AI workspace for real work: research, sales leads, competitor monitoring, reports, files, and follow-up tasks.

No command-line setup first. No token routing first. Open the app, log in, describe the work, and keep the result, process, and files in one project workspace.

<p align="center">
  <img src="assets/screenshots/mycodex-home.jpg" alt="MyCodex desktop workspace" width="900">
</p>

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases/latest">Download</a>
  ·
  <a href="docs/releases/v0.9.6.md">v0.9.6 release notes</a>
  ·
  <a href="#what-you-can-do">What you can do</a>
  ·
  <a href="#screenshots">Screenshots</a>
  ·
  <a href="#feedback">Feedback</a>
</p>

## Download

| Platform | Recommended file | Notes |
| --- | --- | --- |
| macOS Apple Silicon | [`MyCodex-0.9.6-mac-arm64.dmg`](https://github.com/guo2001china/mycodex/releases/download/v0.9.6/MyCodex-0.9.6-mac-arm64.dmg) | M-series Mac |
| macOS Intel | [`MyCodex-0.9.6-mac-x64.dmg`](https://github.com/guo2001china/mycodex/releases/download/v0.9.6/MyCodex-0.9.6-mac-x64.dmg) | Intel Mac |
| Windows x64 | [`MyCodex-0.9.0-win-x64.zip`](https://github.com/guo2001china/mycodex/releases/tag/v0.9.0) | Older archive package; Windows 0.9.6 is pending |

For manual installation, use the DMG. ZIP files in the release are mainly for the desktop updater.

## Why It Matters

Most AI agent tools lose users before the first useful task: API keys, shell commands, model settings, scattered files, and no clear place to continue the work.

MyCodex keeps the whole job together:

- the instruction you gave
- the model and project used
- the execution process
- generated files and previews
- follow-up questions
- WeChat handoff when you leave the computer

The value is simple: less setup, less switching, less lost context.

## What You Can Do

| Workflow | What MyCodex helps with |
| --- | --- |
| Sales leads | Collect public information, summarize context, and produce follow-up tables |
| Competitor monitoring | Check pages, capture changes, and turn observations into notes |
| Operations reports | Pull scattered material into structured weekly or campaign reports |
| Content research | Gather sources, organize themes, and draft reusable outlines |
| File work | Generate Markdown, CSV, HTML, JSON, images, PDFs, and inspect them in the app |
| Browser tasks | Use a desktop-managed browser bridge for workflows that need real page interaction |
| Mobile handoff | Send tasks and receive result files through WeChat |

## v0.9.6

This release makes the desktop app feel more reliable when windows are closed, reopened, minimized, or triggered from login callbacks and external links.

User-visible improvements:

- MyCodex no longer sends login, update, or focus events to a closed desktop window.
- External links and second launches restore a live window when one exists.
- Minimized windows are restored before focus, so the app is easier to find.
- macOS Apple Silicon and Intel installers are refreshed.

Read the full notes: [docs/releases/v0.9.6.md](docs/releases/v0.9.6.md).

## Screenshots

### Start a task

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

Describe the outcome you want, choose a model and project, attach files, or start from a built-in workflow.

### Track the work

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex running task" width="900">

See the task, current step, tool actions, and running state instead of waiting in a blank chat box.

### Keep the result

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result and artifacts" width="900">

The final answer, generated files, attachments, and follow-up context stay in the same conversation.

### Preview files

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Preview Markdown, CSV, HTML, JSON, logs, images, PDFs, and other output before opening or downloading.

### Use it from WeChat

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex WeChat workflow" width="900">

Connect WeChat to send tasks and receive generated files when you are away from the computer.

### Set up models

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription model setup" width="900">

Use subscription-account setup when possible, or configure API Key providers when you need more control.

## Good Fit

- Founders and managers who want research, summaries, and action lists without opening five tools.
- Operators who repeat reporting, content, community, or campaign workflows.
- Sales teams that need structured lead context and follow-up material.
- Assistants and support teams turning messages, files, and webpages into deliverables.
- Non-technical users who want an agent workspace without starting in a terminal.

## Feedback

MyCodex is early. The best feedback is concrete: what job you tried, where you got stuck, and what output you expected.

- [Installation help](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [Bug report](https://github.com/guo2001china/mycodex/issues/new?template=bug_report.yml)
- [Feature request](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [Model provider request](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [Roadmap issues](https://github.com/guo2001china/mycodex/issues?q=is%3Aissue+is%3Aopen+label%3Aroadmap)
- [Discussions](https://github.com/guo2001china/mycodex/discussions)

## Status

MyCodex is currently distributed as packaged installers. Full source is not published in this repository yet.

Test it in a non-critical project first, then move it into workflows where it saves real time.
