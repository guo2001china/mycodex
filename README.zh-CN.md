# MyCodex

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

免费用上 Codex + Hermes，省心、省钱、高效，让你的工作流跑起来不费力。

MyCodex 干的事说白了很简单：把 Codex + Hermes 打包成一个普通人也能顺手用的桌面工作台。

不用提前搞懂 Token 是什么、命令行怎么敲、模型路由怎么配，也不用折腾一堆环境变量。打开 MyCodex，把要做的事说清楚，Agent 自己跑任务、整理过程、输出结果文件。要是需要离开电脑，接上微信，任务进展和成品文件直接发到手机上。

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases">下载 MyCodex</a>
  ·
  <a href="#桌面版完整说明">看桌面版截图</a>
  ·
  <a href="#roadmap-和反馈">Roadmap 和反馈</a>
  ·
  <a href="#加入社群">加入社群</a>
</p>

## 0.6.1 更新亮点

- 连接更稳了：云端认证请求加了明确超时机制，短暂断网之后会自动重试，不会卡死。
- 桌面安装包内置了正式的 MyCodex 云端连接配置，第一次启动不会再误连本地开发地址导致失败。
- Windows 稳定运营链路正式进入 0.6.1：发布流程会自动检查完整的 Windows 压缩包结构、内置 runtime 位置和打包配置。
- macOS Apple Silicon 和 Intel 安装包已同步更新至 0.6.1。
- 微信 + Hermes 依然是主工作流：发任务、跟进对话、拿结果文件，不用守在电脑前。
- 结果不只是一条回复：执行过程、结论、表格、文件和下一步建议，全都留在同一个对话里，随时翻查。
## 0.9.0 发布重点

- 新增真实浏览器控制能力：用户可以从桌面端安装并打开 MyCodex 浏览器扩展，让 Agent 在受控浏览器会话里执行页面操作。
- 控制页新增浏览器插件区域，展示连接状态、活动会话、扩展版本和最近动作。
- 对话输入区新增浏览器工具入口，用于提示 Agent 执行需要真实页面交互的任务。
- 浏览器扩展页面可从桌面端直接打开，不再依赖用户手动查找扩展目录。
- macOS Apple Silicon、macOS Intel 和 Windows x64 安装包已刷新到 0.9.0。
- 微信和 Hermes 仍是主工作流：发任务、继续对话、收结果文件，不用一直守在电脑前。
- 结果不只是一段回复：过程、结论、表格、文件和下一步动作都会留在同一个对话里。

## 解决了什么问题

其实很多人不是不想用 Codex + Hermes，是被前面那关配置给挡回去了。

MyCodex 把门槛压到三步：下载，登录，说任务。跑完以后，结果、过程和文件都留在桌面端；绑定微信之后，手机上也能随时收消息和文件，接着聊。

## 适合哪些人用

- **老板和业务负责人**：在微信里甩一句话，让 MyCodex 帮你整理项目进展、竞品情况、客户信息和待办清单。
- **运营同学**：批量搞定爆款选题、活动复盘、社群话术和内容排期。
- **销售同学**：批量收集线索、补全客户资料、生成跟进建议和汇总表格。
- **助理和客服**：把微信消息、网页资料、零散文件整合成可直接交付的成品。
- **非技术用户**：下载、登录、扫码、发任务，不需要懂 Token、环境变量或命令行。

## 桌面版完整说明

下面逐个介绍桌面版的主要页面。截图里的内容均为示例数据，用来展示真实使用时能看到什么、能操作什么。

### 1. 登录页

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex 登录页" width="900">

打开 MyCodex 后，第一步就是登录。这里刻意做得很克制，不把模型、Token、runtime 这些技术概念一股脑丢给刚上手的用户。

- 手机号验证码登录，简单直接。
- 勾选用户协议和隐私政策。
- 登录过的设备可以自动恢复登录状态。
- 登录服务出现波动时会进入重试，不会只留一个空白窗口让你干等。

先进工作台，再聊模型和任务，这才是普通用户更能接受的节奏。

### 2. 首次接入模型

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex 首次模型接入" width="900">

还没有可用模型时，MyCodex 不会让你自己猜问题出在哪，而是直接把接入入口放在对话区正中间。

- 优先推荐订阅账号方式，省去复制和保存 API Key 的麻烦。
- 同时支持切换为 API Key 方式。
- 可以跳转到完整设置页继续配置。
- 接入成功后自动回到对话主流程。

这一步是为了解决第一次使用时最常见的卡点：软件装好了，但不知道为啥发不了任务。

### 3. 对话主页

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex 对话首页" width="900">

对话页是日常使用最频繁的入口。不用写复杂的提示词，把希望 Agent 交付什么说清楚就行。

- 输入目标任务。
- 选择模型。
- 选择所属项目。
- 添加图片或文件附件。
- 点击内置场景，一键填入提示词。
- 发送任务；执行过程中发现方向不对，随时可以叫停。

内置场景包括：

- 整理热门选题
- 收集销售线索
- 生成运营报告
- 监控竞品动态

这些不是摆样子的演示按钮，而是给不想从零写需求的人提供一个起点。点进去，再改成自己想要的任务就好。

### 4. 项目与历史管理

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex 项目和对话历史管理" width="900">

左侧栏负责把任务收纳整齐。用久了之后，真正需要的是能快速找回某个项目或历史任务，而不是在聊天记录里翻来翻去。

- 主导航：移动版、对话、设置。
- 新建项目。
- 重命名项目。
- 打开项目文件夹。
- 设置为默认项目。
- 删除非默认项目。
- 打开历史对话。
- 删除历史对话。
- 正在运行的对话会显示状态标记，方便回来接着看进展。

项目、对话和本地文件夹是绑定在一起的。以后要找结果，不用全靠脑子记。

### 5. 执行中

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex Agent 执行中" width="900">

Agent 开始跑起来之后，页面会实时展示当前在做什么，不让你对着一个毫无反应的输入框干等。

- 显示用户下达的原始任务。
- 显示 Agent 当前执行的步骤。
- 显示已完成的工具调用动作。
- 左侧历史列表会实时显示运行状态标记。
- 刷新或重新打开窗口后，执行状态和过程事件可以自动恢复。

对等待结果的人来说，这很重要：看到软件在动，心里才踏实。

### 6. 结果与产出文件

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex 对话结果和文件产物" width="900">

任务完成后，结果直接留在对话里。既能看结论，也能看 Agent 生成了哪些文件。

- 展示最终文字结论。
- 支持 Markdown 格式、表格和超链接。
- 保留用户上传的附件。
- 展示 Agent 生成的相关文件。
- 支持继续追问，不用重新交代背景。

这不是用完就丢的聊天框，更像一份可以随时追问、随时翻查的工作记录。

### 7. 查看执行过程

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex 执行过程展开" width="900">

如果对结果不放心，可以把执行过程完整展开来看。

- 查看 Agent 做了哪些操作。
- 查看读取、搜索、汇总、写文件等各个步骤。
- 查看涉及的文件路径。
- 失败、中止、等待用户确认等异常状态会单独高亮显示。

这样至少能回答一个实际问题：Agent 到底干了什么，那个文件是不是它真的生成的。

### 8. 真实浏览器控制

MyCodex 现在可以通过桌面端管理的浏览器扩展，把 Agent 接到真实浏览器会话中。

- 从桌面端安装并打开 MyCodex 浏览器扩展。
- 查看浏览器桥接连接状态、活动会话、扩展版本和最近动作。
- 在对话输入区使用浏览器工具入口，处理需要页面交互的任务。
- 浏览器会话上下文可以进入 Agent 执行链路，同时保留在对话记录中。
- 扩展资源随桌面发布包分发，并使用 Documents 下的稳定安装路径。

### 9. 文件预览

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex 文件预览" width="900">

很多任务最后要的不是一段话，而是一个可以拿走用的文件。MyCodex 把文件预览放在右侧，结果出来后直接点开就能看。

- 点击相关文件即可原地预览。
- 支持纯文本、Markdown、CSV、HTML、JSON、日志、XML 等文本类产物。
- 支持图片预览。
- 支持 PDF 内嵌预览。
- 支持下载文件到本地。
- 支持用系统应用直接打开文件。
- 文件预览面板可以关闭，回到纯对话视图。

先预览，确认没问题再下载或交付，不用来回折腾。

### 9. 移动版（微信接入）
### 10. 移动版

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex 移动版微信入口" width="900">

移动版不是多余的设置项，它是专门为微信使用场景准备的入口。

- 查看个人微信的连接状态。
- 生成登录二维码。
- 展示等待扫码、等待确认、已连接、连接出错等各种状态。
- 随时断开或重新连接。
- 直接在微信里给 MyCodex 发任务。
- 在微信里回复 `1/2/3` 可快速选择菜单操作。
- Agent 生成的结果文件可以直接发回你的微信。
- 右侧提供微信聊天体验预览，所见即所得。

适合"我现在不在电脑前，但想先把任务甩出去"的场景。结果文件回来之后，微信里直接就能拿到，不用再跑回电脑上取。

### 11. 设置页

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex 设置页" width="900">

设置页只放那些不该打扰主流程的内容：账号管理、模型配置、本地运行时。

- 查看登录状态。
- 退出登录。
- 查看模型列表。
- 检测模型是否可用。
- 启用或停用某个模型。
- 设置默认模型。
- 编辑 API Key 模型参数。
- 更换订阅账号绑定的模型。
- 删除模型。
- 查看本地运行时连接地址、版本号、Agent 状态、应用数据目录和结果目录。

日常根本不用常来这里。只有换模型、排查运行问题、退出登录这几种情况才需要打开。

### 12. 订阅账号接入

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex 订阅账号接入" width="900">

新增模型时，默认优先走订阅账号这条路。

- 选择订阅账号。
- 选择模型。
- 发起连接。
- 如果遇到需要网页授权的账号，会自动弹出授权入口。

第一批支持的订阅账号包括：

- Grok 订阅
- Nous Portal
- ChatGPT / Codex
- Gemini OAuth
- MiniMax OAuth
- Qwen Portal
- GitHub Copilot
- GitHub Copilot ACP
- Claude Max

这条路线的目标很明确：让已经买了订阅的人，少复制 Key、少填参数，直接把任务跑起来。

### 13. API Key 接入

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key 接入" width="900">

如果你手头有自己的 API Key，也可以走传统接入方式。

- 选择服务商。
- 选择模型。
- 填写 API Key。
- 填写 Base URL。
- 设置是否作为默认模型。

团队用户和重度用户通常更在意可控性，这个入口保留下来，不强求所有人都走订阅账号。

## 下载

源码暂不对外发布，当前发布打包好的安装包。

当前版本（0.6.1）：

- macOS Apple Silicon：`MyCodex-0.9.0-mac-arm64.dmg` 和 `MyCodex-0.9.0-mac-arm64.zip`。
- macOS Intel：`MyCodex-0.9.0-mac-x64.dmg` 和 `MyCodex-0.9.0-mac-x64.zip`。
- Windows x64：`MyCodex-0.9.0-win-x64.zip`。

请前往 [GitHub Releases](https://github.com/guo2001china/mycodex/releases) 下载。

## Roadmap 和反馈

MyCodex 还在快速迭代中。公开 issue 用来收集路线图投票、安装问题、模型接入需求和翻译修正。

- [Roadmap issues](https://github.com/guo2001china/mycodex/issues?q=is%3Aissue+is%3Aopen+label%3Aroadmap)
- [安装问题反馈](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [功能建议](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [模型接入需求](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [翻译问题反馈](https://github.com/guo2001china/mycodex/issues/new?template=localization.yml)
- [社区讨论](https://github.com/guo2001china/mycodex/discussions)

## 安装使用

**macOS：**

1. Apple Silicon 机器下载 `MyCodex-0.9.0-mac-arm64.dmg`，Intel 机器下载 `MyCodex-0.9.0-mac-x64.dmg`。
2. 打开 dmg。
3. 拖拽安装 `MyCodex.app`。
4. 启动后登录、接入模型、开始发任务。

**Windows：**

1. 等 0.6.1 Windows 资源补齐后，到 Releases 页面下载 Windows x64 portable 包。
2. 解压整个文件夹。
3. 运行解压目录里的 `MyCodex.exe`。

## 加入社群

欢迎加入社群，一起让 MyCodex 用起来更顺手、惠及更多人。

添加时请备注：`MyCodex`

<img src="assets/mycodex-community-wechat.jpg" alt="加入 MyCodex 社群二维码" width="260">

## 当前状态

MyCodex 目前仍是早期预览版本。建议先在测试目录或非核心项目中体验一段时间，再逐步用到重要工作流里。

我们的目标很清晰：让更多普通用户不用折腾 Token、环境配置和命令行，也能稳稳地把 Codex + Hermes 的工作流跑起来。