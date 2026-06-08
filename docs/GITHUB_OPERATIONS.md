# GitHub Operations Checklist

GitHub is the public storefront for DeepSeek企业桌面版. Treat every page as part of the product funnel: search, trust, download, onboarding, feedback, and retention.

## Current Positioning

- Product: DeepSeek企业桌面版 v0.9.68, an enterprise desktop Agent workbench.
- Core jobs: Token sharing, AI skill orders, team model quota sharing, browser tasks, file delivery, and desktop Agent workflows.
- Safety boundary: Token sharing means controlled model invocation capability, quota, and permissions. Do not encourage sending personal keys in plain text.
- Primary conversion: download `DeepSeekDesktop-0.9.68-mac.dmg` or watch releases.
- Secondary conversion: issue feedback, skill-order demand, model-provider request, Token-sharing request, roadmap discussion.

## Page Responsibilities

| Surface | Job |
| --- | --- |
| Repository About | Search keywords, one-line promise, homepage, topics |
| README first screen | Explain DeepSeek企业桌面版, show Token sharing, drive macOS download and release notes |
| Release page | Use title `DeepSeek企业桌面版 v0.9.68`, list assets, known limits, verification |
| Issues | Collect reproducible install bugs, skill-order demand, provider and Token-sharing requests |
| Discussions | Capture broader workflow ideas and community stories |
| Security | Keep secrets out of public reports and point users to official downloads |
| Support | Route users to the right template fast |
| Contributing | Tell people how to help even before full source publication |

## Operating Cadence

- Every release: update Release body, `docs/releases`, README download table, issue template version placeholders, and repo About if positioning changed.
- Every site refresh: make sure GitHub README and 35m.ai use the same brand, current version, macOS downloads, and Windows download.
- Every week: triage open issues, label roadmap signals, reply to install blockers, and close stale duplicate reports.
- Every month: refresh screenshots if the first-run path changed, promote the top 3 roadmap issues, and review topics for search fit.

## Traffic Levers

- Use release titles that include product and version: `DeepSeek企业桌面版 v0.9.68`.
- Keep `DeepSeekDesktop-0.9.68-mac.dmg` visible above the long product tour.
- Convert visitors who are not ready to download: star, watch releases, vote roadmap, request provider, describe a skill order.
- Keep multilingual READMEs in sync for search and trust.
- Do not overclaim source availability. Say packaged installers first until source publication is ready.

## Quality Bar

- No dead links.
- No stale macOS version numbers.
- Windows package status must be explicit; v0.9.68 uses `DeepSeekDesktop-0.9.68-win-x64.zip`.
- Current public copy must use DeepSeek企业桌面版, Token sharing, AI skill orders, and enterprise desktop workbench language.
- Screenshots must show real product surfaces, not generic marketing art.
- Release notes must include downloads, user-visible changes, auto-update status, verification, and known limits.
