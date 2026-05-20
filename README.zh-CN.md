# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

人人都能免费用的 Codex + Hermes，让你的工作流程免 TOKEN、稳定、高效。

MyCodex 做的事情很简单：把 Codex + Hermes 包成一个普通人能直接用的桌面工作台。

你不用先研究 Token、命令行、模型路由和一堆环境变量。打开 MyCodex，说清楚要做什么，Agent 会跑任务、整理过程、生成结果文件。需要离开电脑时，也可以把微信接上，让任务和文件从微信里回来。

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases">下载 MyCodex</a>
  ·
  <a href="#桌面版完整说明">看桌面版截图</a>
  ·
  <a href="#roadmap-和反馈">Roadmap 和反馈</a>
  ·
  <a href="#加入社群">加入社群</a>
</p>

## 0.8.0 发布重点

- 设置页新增 Agent 配置区域，可以调整默认权限、工具范围、网络访问和最长运行时间。
- Runtime 区域增加运行任务状态，可以刷新当前任务并停止全部运行任务。
- Runtime 状态展示 Hermes 数据目录，方便排查本地 Agent 认证和运行环境。
- 对话侧边栏只对运行中、等待、失败和已停止状态展示状态标记；已完成对话不再显示灰色完成勾。
- macOS Apple Silicon 和 Intel 安装包已刷新到 0.8.0。
- 微信和 Hermes 仍是主工作流：发任务、继续对话、收结果文件，不用一直守在电脑前。
- 结果不只是一段回复：过程、结论、表格、文件和下一步动作都会留在同一个对话里。

## 这东西解决什么

大多数人不是不想用 Codex + Hermes，是被前面的配置挡住了。

MyCodex 把入口压到三步：下载，登录，说任务。跑完以后，结果、过程和文件都在桌面端；接了微信以后，手机上也能继续收消息和文件。

## 适合谁

- 老板和负责人：在微信里丢一句话，让 MyCodex 整理进展、竞品、客户和待办。
- 运营同学：批量整理热门选题、活动复盘、社群话术和内容日历。
- 销售同学：收集线索、补齐客户资料、生成跟进建议和汇总表。
- 助理和客服：把零散消息、网页资料和文件整理成可交付结果。
- 不懂技术的人：下载、登录、扫码、发任务，不需要理解 Token、环境变量和命令行。

## 桌面版完整说明

下面把桌面版每个主要页面都展开讲一遍。截图里的内容是示例数据，用来说明真实使用时能看到什么、能点什么。

### 1. 登录页

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex 登录页" width="900">

打开 MyCodex 后，第一步就是登录。这里故意做得很克制，不把模型、Token、runtime 这些东西提前丢给新用户。

- 手机号验证码登录。
- 勾选用户协议和隐私政策。
- 已登录设备可恢复登录态。
- 登录服务异常时会进入重试状态，不会只留一个空白窗口。

先把人带进工作台，再处理模型和任务，这是普通用户更能接受的顺序。

### 2. 首次模型接入

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex 首次模型接入" width="900">

没有可用模型时，MyCodex 不会让用户猜问题出在哪，而是直接把接入入口放在对话区中间。

- 推荐使用订阅账号，减少 API Key 复制和保存成本。
- 支持切换到 API Key 方式。
- 可以进入完整设置页继续配置。
- 接入成功后回到对话主流程。

这一步是为了减少第一次使用时最常见的卡点：下载了软件，但不知道为什么不能发任务。

### 3. 对话首页

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex 对话首页" width="900">

对话页是最常用的入口。用户不用写复杂提示词，只要说清楚希望 Agent 交付什么。

- 输入目标任务。
- 选择模型。
- 选择项目。
- 添加图片或文件附件。
- 点击内置场景快速填入提示。
- 发送任务；执行中如果发现方向不对，可以停止。

内置场景包括：

- 整理热门选题。
- 收集销售线索。
- 生成运营报告。
- 监控竞品变化。

这些场景不是演示按钮，而是给不想从零写需求的人一个起点。先点一个，再改成自己的任务就行。

### 4. 项目和历史管理

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex 项目和对话历史管理" width="900">

左侧栏负责把任务收纳起来。用久以后，用户真正需要的是能快速回到某个项目、某个历史任务，而不是在聊天记录里翻半天。

- 主导航：移动版、对话、设置。
- 新建项目。
- 重命名项目。
- 打开项目文件夹。
- 设置默认项目。
- 删除非默认项目。
- 打开历史对话。
- 删除历史对话。
- 运行中的对话会显示状态标记，方便回来继续看。

项目、对话和文件夹是绑在一起的。以后找结果，不用靠记忆。

### 5. 执行中页面

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex Agent 执行中" width="900">

Agent 开始跑以后，页面会告诉用户现在正在做什么。

- 展示用户原始任务。
- 展示 Agent 当前执行步骤。
- 展示已执行的工具动作。
- 执行中的对话在左侧历史里有状态提示。
- 刷新或重新打开窗口后，可以恢复运行状态和过程事件。

这对等结果的人很重要：他需要看到软件在动，而不是盯着一个不知道有没有反应的输入框。

### 6. 结果和产物

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex 对话结果和文件产物" width="900">

任务完成后，结果直接留在对话里。能看结论，也能看到 Agent 生成了哪些文件。

- 展示最终文字结论。
- 支持 Markdown、表格和链接。
- 保留用户上传的附件。
- 展示 Agent 生成的相关文件。
- 支持继续追问，不需要重新描述上下文。

这不是一次性的聊天框，更接近一份能继续追问、能回头查的工作记录。

### 7. 执行过程展开

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex 执行过程展开" width="900">

如果用户不放心结果，可以把执行过程展开看。

- 查看 Agent 做过哪些操作。
- 查看读取、搜索、汇总、写文件等步骤。
- 查看涉及文件路径。
- 失败、终止、等待用户确认等状态会单独显示。

这样至少能回答一个现实问题：Agent 到底做了什么，文件是不是它真的生成的。

### 8. Agent 设置和 Runtime 控制

MyCodex 现在把 Agent 运行方式和可用范围交给用户直接控制。

- 设置默认 Agent 权限、工具范围、网络访问和最长运行时间。
- 在设置页查看当前 Runtime 运行任务。
- 刷新当前任务状态，或停止全部运行任务。
- 查看 Hermes 数据目录，用于本地认证和运行环境排查。
- Agent 产物写入当前项目下的 per-run 目录，项目工作目录和结果目录更清楚。

### 9. 文件预览

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex 文件预览" width="900">

很多任务最后都不是要一句话，而是要一个文件。MyCodex 把文件预览放在右侧，结果出来后可以直接点开看。

- 点击相关文件即可预览。
- 支持文本、Markdown、CSV、HTML、JSON、日志、XML 等文本型产物。
- 支持图片预览。
- 支持 PDF 内嵌预览。
- 支持下载文件。
- 支持用系统应用打开文件。
- 文件预览面板可关闭，回到纯对话视图。

用户可以先看，确认没问题再下载或用系统应用打开。

### 10. 移动版

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex 移动版微信入口" width="900">

移动版不是另一个设置项，它是给微信使用场景准备的入口。

- 查看个人微信连接状态。
- 生成登录二维码。
- 展示等待扫码、等待确认、已连接、错误等状态。
- 断开连接或重新连接。
- 在微信里直接给 MyCodex 发任务。
- 微信回复 `1/2/3` 可选择菜单操作。
- Agent 生成的结果文件可以直接发回微信。
- 右侧提供微信聊天体验预览。

适合那种“我现在不在电脑前，但想先把任务丢出去”的场景。结果文件回来以后，也能直接在微信里拿到。

### 11. 设置页

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex 设置页" width="900">

设置页只放那些不应该打扰主流程的东西：账号、模型、本地运行时。

- 查看登录状态。
- 退出登录。
- 查看模型列表。
- 检测模型是否可用。
- 启用或停用模型。
- 设置默认模型。
- 编辑 API Key 模型。
- 更换订阅账号模型。
- 删除模型。
- 查看本地运行时连接地址、版本、Agent 状态、应用数据目录和结果目录。

日常使用不需要天天来这里。只有换模型、查运行状态、退出登录时才需要打开。

### 12. 订阅账号接入

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex 订阅账号接入" width="900">

新增模型时，默认先给订阅账号路线。

- 选择订阅账号。
- 选择模型。
- 发起连接。
- 遇到需要网页登录授权的账号，会提供授权入口。

第一批订阅账号入口包括：

- Grok 订阅。
- Nous Portal。
- ChatGPT / Codex。
- Gemini OAuth。
- MiniMax OAuth。
- Qwen Portal。
- GitHub Copilot。
- GitHub Copilot ACP。
- Claude Max。

这条路线的目标很明确：让已经买了订阅的人，少复制 Key、少填参数，先把任务跑起来。

### 13. API Key 接入

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key 接入" width="900">

如果你有自己的 API Key，也可以走传统接入方式。

- 选择供应商。
- 选择模型。
- 填写 API Key。
- 填写 Base URL。
- 设置是否默认模型。

团队和重度用户通常更在意可控性，这个入口保留下来，不强迫所有人都走订阅账号。

## 下载

源码暂不发布，先发布打包后的安装包。

当前 Release：

- macOS Apple Silicon：`MyCodex-0.8.0-mac-arm64.dmg` 和 `MyCodex-0.8.0-mac-arm64.zip`。
- macOS Intel：`MyCodex-0.8.0-mac-x64.dmg` 和 `MyCodex-0.8.0-mac-x64.zip`。
- Windows x64：`MyCodex-0.8.0-win-x64.zip`。

请到 [GitHub Releases](https://github.com/guo2001china/mycodex/releases) 下载。

## Roadmap 和反馈

MyCodex 还在快速迭代。公开 issue 会用来收集路线图投票、安装问题、模型接入需求和翻译修正。

- [Roadmap issues](https://github.com/guo2001china/mycodex/issues?q=is%3Aissue+is%3Aopen+label%3Aroadmap)
- [安装问题](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [功能建议](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [模型接入需求](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [翻译反馈](https://github.com/guo2001china/mycodex/issues/new?template=localization.yml)
- [Discussions](https://github.com/guo2001china/mycodex/discussions)

## 使用

macOS：

1. Apple Silicon 机器下载 `MyCodex-0.8.0-mac-arm64.dmg`，Intel 机器下载 `MyCodex-0.8.0-mac-x64.dmg`。
2. 打开 dmg。
3. 拖拽安装 `MyCodex.app`。
4. 启动后登录、接入模型、开始发任务。

Windows：

1. 到 Releases 下载 `MyCodex-0.8.0-win-x64.zip`。
2. 解压整个文件夹。
3. 运行解压目录里的 `MyCodex.exe`。

## 加入社群

加入社群，让 MyCodex 更普惠。

扫码添加时请备注：`MyCodex`

<img src="assets/mycodex-community-wechat.jpg" alt="加入 MyCodex 社群二维码" width="260">

## 当前状态

MyCodex 仍是早期预览版。建议先在测试目录或非关键项目中体验，再逐步放到重要工作流里。

我们的目标很明确：让更多普通用户不用折腾 Token、环境和命令行，也能稳定使用 Codex + Hermes 的工作流。
