# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

Free Codex + Hermes for everyone: fewer tokens, fewer fragile setups, a steadier workflow.

MyCodex wraps Codex + Hermes into a desktop workspace that normal users can actually open and use.

You do not need to start with tokens, command lines, model routing, or environment variables. Open MyCodex, describe the result you want, and let the Agent run the task, show the process, and save the output files. When you need to step away from the computer, connect WeChat and let tasks and files come back through your phone.

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases">Download MyCodex</a>
  ·
  <a href="#desktop-tour">Desktop tour</a>
  ·
  <a href="#roadmap-and-feedback">Roadmap</a>
  ·
  <a href="#community">Community</a>
</p>

## v0.6.1 Highlights

- Connection stability is better: cloud auth requests now have explicit timeouts and safe retry behavior for short network failures.
- Downloadable desktop packages now carry the production MyCodex cloud connection config, reducing first-run failures caused by local development defaults.
- Windows stable-operation work is in this release line: the release pipeline now checks full Windows zip structure, bundled runtime placement, and packaged config before a Windows build is attached.
- macOS Apple Silicon and Intel packages are refreshed for 0.6.1.
- WeChat and Hermes remain the main workflow: send tasks, continue conversations, and receive result files without staying at your desk.
- Results are more than chat replies: process, conclusions, tables, files, and next steps stay in the same conversation.

## What It Solves

Many people want Codex + Hermes, but they drop off before the first useful task because setup gets in the way.

MyCodex reduces the entry path to three steps: download, log in, describe the task. The result, process, and generated files stay in the desktop app. After WeChat is connected, the phone can also send tasks and receive files.

## Who It Is For

- Founders and managers: send one message and get progress summaries, competitor notes, customer context, and action items.
- Operators: collect topics, draft campaign reviews, prepare community messages, and build content calendars.
- Sales teams: gather leads, enrich customer context, generate follow-up suggestions, and export tables.
- Assistants and support teams: turn scattered messages, webpages, and files into usable deliverables.
- Non-technical users: download, log in, scan, send tasks, and avoid tokens, shell commands, and environment setup.

## Desktop Tour

The screenshots below use example data. They show what users can see and click in the desktop app.

### 1. Login

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex login page" width="900">

MyCodex starts with login before it asks users to think about models or runtime details.

- Phone verification-code login.
- User agreement and privacy policy checkbox.
- Session restore on already logged-in devices.
- Retry state when the login service is unavailable.

The order matters: get users into the workspace first, then handle models and tasks.

### 2. First Model Setup

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex first model setup" width="900">

When no usable model exists, MyCodex shows the setup entry directly inside the conversation area.

- Subscription-account setup is recommended.
- API Key setup is still available.
- Users can open the full settings page if they need more control.
- After setup, the app returns to the conversation flow.

This removes a common first-run failure: the app is installed, but the user has no idea why tasks cannot be sent.

### 3. Conversation Home

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex conversation home" width="900">

Conversation is the main workspace. Users only need to say what they want the Agent to deliver.

- Type the task goal.
- Choose a model.
- Choose a project.
- Attach images or files.
- Start from built-in task scenarios.
- Send the task; stop it if the direction is wrong.

Built-in scenarios:

- Collect trending topics.
- Gather sales leads.
- Generate an operations report.
- Monitor competitor changes.

These are not demo buttons. They are starting points for users who do not want to write a task from scratch.

### 4. Projects and History

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex projects and conversation history" width="900">

The sidebar keeps tasks organized. After a few days of use, users need to get back to a project or past task quickly instead of digging through chat history.

- Main navigation: Mobile, Conversation, Settings.
- Create projects.
- Rename projects.
- Open project folders.
- Set the default project.
- Delete non-default projects.
- Open conversation history.
- Delete conversations.
- See running-state markers in the conversation list.

Projects, conversations, and folders stay tied together, so results are easier to find later.

### 5. Running Tasks

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex Agent running" width="900">

When the Agent starts working, the page shows what is happening.

- User task remains visible.
- Current Agent step is shown.
- Tool actions are displayed.
- Running conversations show a status marker in the sidebar.
- Process state can be restored after refresh or reopening the window.

Users need to see that the app is moving, not stare at an input box with no feedback.

### 6. Results and Artifacts

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex result and artifacts" width="900">

Completed tasks stay in the same conversation. Users can read the answer and see which files the Agent created.

- Final text result.
- Markdown, tables, and links.
- Uploaded attachments.
- Generated result files.
- Follow-up questions without restating the full context.

This makes a conversation closer to a work record than a throwaway chat.

### 7. Execution Details

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex execution details" width="900">

If the user wants to check the work, the execution process can be expanded.

- See what the Agent did.
- Review read, search, summarize, and write-file steps.
- See touched file paths.
- Failed, stopped, and waiting states are shown separately.

This answers a practical question: what did the Agent actually do?

### 8. File Preview

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex file preview" width="900">

Many tasks end with a file, not just a paragraph. MyCodex puts file preview on the right side so users can open results immediately.

- Click related files to preview them.
- Preview text, Markdown, CSV, HTML, JSON, logs, XML, and other text artifacts.
- Preview images.
- Preview PDFs inline.
- Download files.
- Open files with the system app.
- Close the preview panel and return to conversation-only mode.

Users can inspect the output before downloading it or opening it elsewhere.

### 9. Mobile

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex mobile WeChat entry" width="900">

Mobile is the WeChat entry point, not just another settings screen.

- Check personal WeChat connection status.
- Generate a login QR code.
- Show waiting-for-scan, waiting-for-confirmation, connected, and error states.
- Disconnect or reconnect.
- Send tasks to MyCodex from WeChat.
- Reply with `1/2/3` to choose menu actions.
- Receive generated files back in WeChat.
- Preview the WeChat chat experience on the right.

This is useful when a user is away from the computer but wants to send a task now.

### 10. Settings

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex settings" width="900">

Settings only contains things that should not interrupt the main workflow: account, models, and local runtime.

- View login state.
- Log out.
- View model list.
- Check whether a model works.
- Enable or disable models.
- Set the default model.
- Edit API Key models.
- Replace subscription-account models.
- Delete models.
- View local runtime URL, version, Agent status, app data directory, and results directory.

Most users only come here when changing models, checking runtime state, or logging out.

### 11. Subscription Account Setup

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex subscription account setup" width="900">

New model setup starts with the subscription-account path.

- Choose a subscription account.
- Choose a model.
- Start the connection.
- If web authorization is required, MyCodex provides the authorization link.

First subscription entries include:

- Grok subscription.
- Nous Portal.
- ChatGPT / Codex.
- Gemini OAuth.
- MiniMax OAuth.
- Qwen Portal.
- GitHub Copilot.
- GitHub Copilot ACP.
- Claude Max.

The goal is simple: users who already pay for a subscription should not have to copy keys and tune parameters before running a task.

### 12. API Key Setup

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key setup" width="900">

If you already have your own API Key, the traditional setup path is still available.

- Choose a provider.
- Choose a model.
- Enter the API Key.
- Enter Base URL.
- Decide whether it should be the default model.

Teams and power users often need this control, so the API Key path remains available.

## Download

Source code is not published yet. This repository currently provides packaged installers first.

Current release:

- macOS Apple Silicon: `MyCodex-0.6.1-mac-arm64.dmg` or `MyCodex-0.6.1-mac-arm64.zip`.
- macOS Intel: `MyCodex-0.6.1-mac-x64.dmg` or `MyCodex-0.6.1-mac-x64.zip`.
- Windows x64: 0.6.1 includes Windows stability work, but the downloadable Windows zip still needs a target-OS runtime build. Use the historical portable package for now; the 0.6.1 Windows asset will be attached after that build is ready.

Download from [GitHub Releases](https://github.com/guo2001china/mycodex/releases).

## Roadmap and Feedback

MyCodex is still moving quickly. Public issues are used for roadmap signals, install problems, model-provider requests, and translation fixes.

- [Roadmap issues](https://github.com/guo2001china/mycodex/issues?q=is%3Aissue+is%3Aopen+label%3Aroadmap)
- [Installation help](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [Feature request](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [Model provider request](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [Translation feedback](https://github.com/guo2001china/mycodex/issues/new?template=localization.yml)
- [Discussions](https://github.com/guo2001china/mycodex/discussions)

## Install

macOS:

1. Apple Silicon users download `MyCodex-0.6.1-mac-arm64.dmg`; Intel users download `MyCodex-0.6.1-mac-x64.dmg`.
2. Open the dmg.
3. Drag `MyCodex.app` into Applications.
4. Launch, log in, connect a model, and start sending tasks.

Windows:

1. Download the Windows x64 portable package from Releases when the 0.6.1 Windows asset is attached.
2. Extract the whole folder.
3. Run `MyCodex.exe`.

## Community

Join the community and help make MyCodex more accessible.

When adding the community contact, please write: `MyCodex`

<img src="assets/mycodex-community-wechat.jpg" alt="Join the MyCodex community QR code" width="260">

## Status

MyCodex is still an early preview. Try it in a test folder or non-critical workflow first, then move it into more important work once it fits your process.

The goal is clear: let more people use Codex + Hermes without fighting tokens, environments, and command lines.
