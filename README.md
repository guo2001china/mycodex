# MyCodex

人人都能免费用的 Codex + Hermes，让你的工作流程免 TOKEN、稳定、高效。

MyCodex 不是让用户学习 AI 概念的工具。它更像一个桌面工作台：用户说清楚要交付什么，MyCodex 负责调度 Agent、Hermes、本地运行时、文件和移动入口，最后把结果放回对话里。

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases">下载 MyCodex</a>
  ·
  <a href="#桌面版完整说明">看桌面版截图</a>
  ·
  <a href="#加入社群">加入社群</a>
</p>

## 0.5.0 发布重点

- 微信管理 MyCodex：在微信里发任务、继续对话、接收结果文件，不用一直守在电脑前。
- 微信管理 Hermes：把 Hermes 的执行能力接进 MyCodex 工作流，用户只需要用聊天方式调度 Agent。
- 自动化控制电脑和手机：适合重复点击、跨页面整理、浏览器访问、手机消息入口和人机协作流程。
- 隐私浏览器方向：把登录、访问、自动化浏览和账号隔离放进更可控的环境，减少主浏览器污染。
- 模型接入更简单：推荐订阅账号接入，少复制 API Key；也保留 API Key 给高级用户。
- 结果更像交付物：过程、结论、表格、文件和下一步动作都在同一个对话里。

## 用户为什么会用

普通用户不会关心 Token、模型路由、Hermes、runtime 或命令行。他们只关心三件事：

1. 能不能下载就用。
2. 能不能一句话交代任务。
3. 能不能直接拿到结果和文件。

MyCodex 的主路径就是围绕这三点设计的。

## 适合谁

- 老板和负责人：在微信里丢一句话，让 MyCodex 整理进展、竞品、客户和待办。
- 运营同学：批量整理热门选题、活动复盘、社群话术和内容日历。
- 销售同学：收集线索、补齐客户资料、生成跟进建议和汇总表。
- 助理和客服：把零散消息、网页资料和文件整理成可交付结果。
- 不懂技术的人：下载、登录、扫码、发任务，不需要理解 Token、环境变量和命令行。

## 桌面版完整说明

以下截图展示桌面版核心页面和功能。示例数据用于说明产品能力。

### 1. 登录页

<img src="assets/screenshots/desktop-login.jpg" alt="MyCodex 登录页" width="900">

用户打开 MyCodex 后先进入登录门禁。

- 手机号验证码登录。
- 勾选用户协议和隐私政策。
- 已登录设备可恢复登录态。
- 登录服务异常时会进入重试状态，避免用户看到空白页。

价值：普通用户不用配置环境，也不用先理解模型和 Token，先完成账号进入工作台。

### 2. 首次模型接入

<img src="assets/screenshots/desktop-model-setup.jpg" alt="MyCodex 首次模型接入" width="900">

如果还没有默认模型，MyCodex 会直接引导用户完成模型接入。

- 推荐使用订阅账号，减少 API Key 复制和保存成本。
- 支持切换到 API Key 方式。
- 可以进入完整设置页继续配置。
- 接入成功后自动回到对话主流程。

价值：新用户不会卡在“为什么不能发任务”，页面会明确告诉他下一步做什么。

### 3. 对话首页

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="MyCodex 对话首页" width="900">

对话是 MyCodex 的默认工作区。用户只需要描述想要的交付结果。

- 输入目标任务。
- 选择模型。
- 选择项目。
- 添加图片或文件附件。
- 点击内置场景快速填入提示。
- 发送任务，执行中可停止。

内置场景包括：

- 整理热门选题。
- 收集销售线索。
- 生成运营报告。
- 监控竞品变化。

价值：用户不用学提示词，从常见业务场景开始就能跑。

### 4. 项目和历史管理

<img src="assets/screenshots/desktop-project-history.jpg" alt="MyCodex 项目和对话历史管理" width="900">

左侧栏负责把任务整理成项目和历史对话。

- 主导航：移动版、对话、设置。
- 新建项目。
- 重命名项目。
- 打开项目文件夹。
- 设置默认项目。
- 删除非默认项目。
- 打开历史对话。
- 删除历史对话。
- 运行中的对话会显示状态标记。

价值：用户不需要翻聊天记录，也不需要记文件在哪个目录，项目、对话和结果天然归档。

### 5. 执行中页面

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="MyCodex Agent 执行中" width="900">

Agent 执行任务时，页面会持续展示过程状态。

- 展示用户原始任务。
- 展示 Agent 当前执行步骤。
- 展示已执行的工具动作。
- 执行中的对话在左侧历史里有状态提示。
- 刷新或重新打开窗口后，可以恢复运行状态和过程事件。

价值：用户知道 MyCodex 还在工作，不会误以为卡死。

### 6. 结果和产物

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="MyCodex 对话结果和文件产物" width="900">

任务完成后，结果会留在同一个对话里。

- 展示最终文字结论。
- 支持 Markdown、表格和链接。
- 保留用户上传的附件。
- 展示 Agent 生成的相关文件。
- 支持继续追问，不需要重新描述上下文。

价值：对话不是临时聊天，而是一个可追溯的工作交付记录。

### 7. 执行过程展开

<img src="assets/screenshots/desktop-execution-process.jpg" alt="MyCodex 执行过程展开" width="900">

用户需要追查过程时，可以展开执行记录。

- 查看 Agent 做过哪些操作。
- 查看读取、搜索、汇总、写文件等步骤。
- 查看涉及文件路径。
- 失败、终止、等待用户确认等状态会单独显示。

价值：结果不是黑盒，用户能判断 Agent 做得是否靠谱。

### 8. 文件预览

<img src="assets/screenshots/desktop-file-preview.jpg" alt="MyCodex 文件预览" width="900">

右侧文件预览让结果文件不用离开 MyCodex 就能查看。

- 点击相关文件即可预览。
- 支持文本、Markdown、CSV、HTML、JSON、日志、XML 等文本型产物。
- 支持图片预览。
- 支持 PDF 内嵌预览。
- 支持下载文件。
- 支持用系统应用打开文件。
- 文件预览面板可关闭，回到纯对话视图。

价值：用户拿到的是文件和内容，不是只有一段聊天回复。

### 9. 移动版

<img src="assets/screenshots/desktop-mobile-weixin.jpg" alt="MyCodex 移动版微信入口" width="900">

移动版是微信个人号入口。

- 查看个人微信连接状态。
- 生成登录二维码。
- 展示等待扫码、等待确认、已连接、错误等状态。
- 断开连接或重新连接。
- 在微信里直接给 MyCodex 发任务。
- 微信回复 `1/2/3` 可选择菜单操作。
- Agent 生成的结果文件可以直接发回微信。
- 右侧提供微信聊天体验预览。

价值：用户可以在微信里派活和收文件，适合不想一直盯桌面的场景。

### 10. 设置页

<img src="assets/screenshots/desktop-settings.jpg" alt="MyCodex 设置页" width="900">

设置页只放深层配置，不打扰对话主流程。

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

价值：普通用户只在需要时进入设置；日常使用只看对话、项目、移动版和结果。

### 11. 订阅账号接入

<img src="assets/screenshots/desktop-model-subscription.jpg" alt="MyCodex 订阅账号接入" width="900">

新增模型默认推荐订阅账号。

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

价值：让更多人不再被 API Key 和 Token 成本挡住。

### 12. API Key 接入

<img src="assets/screenshots/desktop-model-api-key.jpg" alt="MyCodex API Key 接入" width="900">

高级用户仍然可以用 API Key 接入。

- 选择供应商。
- 选择模型。
- 填写 API Key。
- 填写 Base URL。
- 设置是否默认模型。

价值：保留可控性，团队和重度用户可以继续使用自己的模型供应商。

## 下载

源码暂不发布，先发布打包后的安装包。

当前 Release：

- macOS Apple Silicon：`MyCodex-0.5.0-mac-arm64.dmg` 和 `MyCodex-0.5.0-mac-arm64.zip`。
- Windows x64：当前可用 portable 包仍在历史 Release 中，0.5.0 Windows 包会继续补齐。

请到 [GitHub Releases](https://github.com/guo2001china/mycodex/releases) 下载。

## 使用

macOS：

1. 下载 `MyCodex-0.5.0-mac-arm64.dmg`。
2. 打开 dmg。
3. 拖拽安装 `MyCodex.app`。
4. 启动后登录、接入模型、开始发任务。

Windows：

1. 到 Releases 下载 Windows x64 portable 包。
2. 解压整个文件夹。
3. 运行解压目录里的 `MyCodex.exe`。

## 加入社群

加入社群，让 MyCodex 更普惠。

扫码添加时请备注：`MyCodex`

<img src="assets/mycodex-community-wechat.jpg" alt="加入 MyCodex 社群二维码" width="260">

## 当前状态

MyCodex 仍是早期预览版。建议先在测试目录或非关键项目中体验，再用于重要工作流。

我们的目标很明确：让更多普通用户不用折腾 Token、环境和命令行，也能稳定使用 Codex + Hermes 的工作流。
