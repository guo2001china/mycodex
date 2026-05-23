# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

MyCodex 把 Codex + Hermes 变成一个普通人能直接用的桌面 AI 工作台：调研、销售线索、竞品监控、运营报告、文件产出、后续跟进，都放在一个项目里。

不用先研究命令行、Token、模型路由和环境变量。打开应用，登录，说清楚要做什么，MyCodex 会保留任务、过程、结果和文件。

<p align="center">
  <img src="assets/screenshots/mycodex-home.jpg" alt="MyCodex 桌面工作台" width="900">
</p>

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases/latest">下载</a>
  ·
  <a href="docs/releases/v0.9.7.md">v0.9.7 发布说明</a>
  ·
  <a href="#能做什么">能做什么</a>
  ·
  <a href="#产品截图">产品截图</a>
  ·
  <a href="#反馈">反馈</a>
</p>

## 下载

| 平台 | 推荐文件 | 说明 |
| --- | --- | --- |
| macOS Apple Silicon | [`MyCodex-0.9.7-mac-arm64.dmg`](https://github.com/guo2001china/mycodex/releases/download/v0.9.7/MyCodex-0.9.7-mac-arm64.dmg) | M 系列 Mac |
| macOS Intel | [`MyCodex-0.9.7-mac-x64.dmg`](https://github.com/guo2001china/mycodex/releases/download/v0.9.7/MyCodex-0.9.7-mac-x64.dmg) | Intel Mac |
| Windows x64 | [`MyCodex-0.9.0-win-x64.zip`](https://github.com/guo2001china/mycodex/releases/tag/v0.9.0) | 历史包；Windows 0.9.7 等待 runtime 构建刷新 |

手动安装优先下载 DMG。Release 里的 ZIP 主要给桌面自动更新使用。

## 价值

很多 AI Agent 工具的问题不是能力不够，而是用户还没跑出第一件有用的事，就被 API Key、命令行、模型配置、文件散落和上下文丢失挡住了。

MyCodex 把一件工作放回同一个地方：

- 你发出的任务
- 使用的模型和项目
- Agent 的执行过程
- 生成的文件和预览
- 后续追问
- 离开电脑后的微信接力

核心价值很直接：少配置、少切换、少丢上下文。

## 能做什么

| 场景 | MyCodex 帮你做什么 |
| --- | --- |
| 销售线索 | 收集公开信息、整理客户背景、生成跟进表 |
| 竞品监控 | 查看页面变化，把观察整理成可复查的记录 |
| 运营报告 | 把零散资料整理成周报、活动复盘、指标说明 |
| 内容调研 | 收集来源、归纳主题、生成可复用大纲 |
| 文件工作 | 生成 Markdown、CSV、HTML、JSON、图片、PDF，并在应用里预览 |
| 浏览器任务 | 通过桌面管理的浏览器桥接处理需要真实页面交互的流程 |
| 微信接力 | 离开电脑后继续发任务、收文件 |

## v0.9.7

这一版重点把 Agent 产物变成用户能直接检查和复用的文件，同时让本地模型用户能在应用里调整运行参数。

用户能感知到的变化：

- 本地模型设置新增运行参数入口，可以直接调整 `llama-server` 启动参数。
- Agent 生成的截图、图片、PDF、Office 文档等产物会进入附件和预览，不再把 base64 长串塞进聊天正文。
- 执行过程里的产物卡片可以复用右侧预览面板，用户不用离开对话就能检查文件。
- 订阅账号和本地模型状态展示更清楚，加载失败时会在设置页暴露原因。
- macOS Apple Silicon 和 Intel 安装包已刷新，桌面端自动更新元数据已发布。

完整发布说明：[docs/releases/v0.9.7.md](docs/releases/v0.9.7.md)。

## 产品截图

### 发起任务

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex 对话首页" width="900">

说清楚想要什么结果，选择模型和项目，附加文件，或者从内置工作流开始。

### 看执行过程

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex 执行中" width="900">

任务、当前步骤、工具动作和运行状态都在页面里，不用盯着空白聊天框等。

### 留住结果

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex 结果和文件" width="900">

结论、生成文件、附件和后续追问上下文都留在同一个对话里。

### 预览文件

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex 文件预览" width="900">

Markdown、CSV、HTML、JSON、日志、图片、PDF 等结果可以先预览，再决定下载或打开。

### 微信接力

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex 微信工作流" width="900">

接入微信后，离开电脑也能继续发任务、收文件。

### 接入模型

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex 订阅账号模型接入" width="900">

优先用订阅账号减少 API Key 配置；需要更强控制时，也可以使用 API Key 方式。

## 适合谁

- 老板和负责人：少开几个工具，直接拿调研、总结和行动清单。
- 运营同学：重复做报告、选题、社群、活动复盘时少复制粘贴。
- 销售团队：把线索背景和跟进素材整理成结构化结果。
- 助理和客服：把消息、文件、网页变成可交付内容。
- 不懂技术的人：不用先学命令行，也能跑 Agent 工作流。

## 反馈

MyCodex 还在早期。最有价值的反馈是具体的：你想完成什么工作，卡在哪一步，希望最后得到什么结果。

- [安装问题](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [Bug 反馈](https://github.com/guo2001china/mycodex/issues/new?template=bug_report.yml)
- [功能建议](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [模型接入需求](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [Roadmap issues](https://github.com/guo2001china/mycodex/issues?q=is%3Aissue+is%3Aopen+label%3Aroadmap)
- [Discussions](https://github.com/guo2001china/mycodex/discussions)

## 当前状态

MyCodex 当前以打包安装包形式发布，完整源码暂未在这个仓库公开。

建议先在非关键项目里试用；确认适合你的流程后，再放进真正节省时间的工作里。
