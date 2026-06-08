# Security Policy

DeepSeek企业桌面版 is distributed as packaged installers. Source code is not published in this repository yet.

Please do not post API keys, tokens, cookies, account credentials, private files, or private logs in public issues.

## Token Sharing Boundary

Token sharing means controlled model invocation capability, quota, and permissions. It does not mean distributing personal keys in plain text. If your report involves team model capacity, describe the permission model and failure mode without revealing secrets.

## Reporting

If you find a security problem, open a GitHub issue with a high-level description only and remove all secrets. If the report needs private details, say that in the issue so we can move the conversation to a safer channel.

## Installer Trust

Download DeepSeek企业桌面版 only from the official GitHub Releases page:

https://github.com/guo2001china/mycodex/releases

For macOS v0.9.68, prefer `DeepSeekDesktop-0.9.68-mac.dmg` for manual installation. ZIP assets are attached mainly for the desktop updater. Windows is currently marked as an older archive package.

Current release notes:

https://github.com/guo2001china/mycodex/blob/main/docs/releases/v0.9.68.md

## Current Status

DeepSeek企业桌面版 is an early enterprise desktop Agent workbench. Test it in non-critical workflows first, especially before connecting shared model capacity or customer-sensitive tasks.
