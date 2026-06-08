# DeepSeek企业桌面版

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md)

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Release" src="https://img.shields.io/github/v/release/guo2001china/mycodex?display_name=tag"></a>
  <a href="https://github.com/guo2001china/mycodex/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/guo2001china/mycodex/total"></a>
  <a href="https://github.com/guo2001china/mycodex/issues"><img alt="Issues" src="https://img.shields.io/github/issues/guo2001china/mycodex"></a>
  <a href="https://github.com/guo2001china/mycodex/discussions"><img alt="Discussions" src="https://img.shields.io/badge/discussions-open-2ea44f"></a>
</p>

DeepSeek企业桌面版 v0.9.68 把 **Token共享**、**AI 技能接单** 和 **桌面 Agent 交付流程** 放进一个企业工作台。

团队不用到处发 Key，不用重复买额度，也不用让每个人重新配置模型。共享的是可控调用能力、额度和权限边界，不鼓励明文散发个人密钥。

<p align="center">
  <img src="assets/screenshots/mycodex-home.jpg" alt="DeepSeek企业桌面版桌面 Agent 工作台" width="900">
</p>

<p align="center">
  <a href="https://github.com/guo2001china/mycodex/releases/download/v0.9.68/DeepSeekDesktop-0.9.68-mac.dmg">下载 macOS DMG</a>
  ·
  <a href="docs/releases/v0.9.68.md">v0.9.68 发布说明</a>
  ·
  <a href="#ai-技能接单">AI 技能接单</a>
  ·
  <a href="#反馈">反馈</a>
</p>

## 下载

| 平台 | 推荐文件 | 说明 |
| --- | --- | --- |
| macOS universal | [`DeepSeekDesktop-0.9.68-mac.dmg`](https://github.com/guo2001china/mycodex/releases/download/v0.9.68/DeepSeekDesktop-0.9.68-mac.dmg) | 当前 v0.9.68 安装包，适合 Apple Silicon 和 Intel Mac |
| macOS updater | [`DeepSeekDesktop-0.9.68-mac.zip`](https://github.com/guo2001china/mycodex/releases/download/v0.9.68/DeepSeekDesktop-0.9.68-mac.zip) | 主要给自动更新使用 |
| Windows x64 | [`MyCodex-0.9.0-win-x64.zip`](https://github.com/guo2001china/mycodex/releases/tag/v0.9.0) | 历史归档包；Windows v0.9.68 等待 runtime 验证 |

手动安装优先下载 DMG。发布资产技术名保留 `DeepSeekDesktop`，用户可见品牌使用 `DeepSeek企业桌面版`。

## Token共享

Token共享不是把个人密钥明文发给团队成员，而是把可控模型调用能力接进桌面端。

- 统一接入模型账号、API Key、本地模型或订阅额度。
- 团队成员使用授权能力跑技能，不需要每个人重复配置模型。
- 任务历史、执行过程、工具动作和结果文件留在桌面项目里。
- 登录、付款、删除、发送、发布和客户敏感动作保留人工确认。

## AI 技能接单

| 技能 | DeepSeek企业桌面版帮你交付什么 |
| --- | --- |
| 销售线索 | 收集公开公司信息、联系人线索、来源说明和跟进表 |
| 运营报告 | 把零散资料、截图和数据整理成周报、复盘和行动清单 |
| 竞品监控 | 跟踪公开产品、价格、招聘和发布变化 |
| 客服工单 | 分类问题、草拟回复、总结上下文，并保留确认点 |
| 招聘筛选 | 对照岗位要求整理简历和初筛记录 |
| 会议纪要 | 把会议输入转换成决策、任务和后续文件 |
| 浏览器任务 | 读取网页、收集来源、辅助填表，并输出结构化文件 |

## v0.9.68

Release title：**DeepSeek企业桌面版 v0.9.68**。

这一版把 GitHub 门面、官网、下载资产和 SEO 文案统一到新版企业桌面定位。

- 公开品牌升级为 DeepSeek企业桌面版。
- 当前 macOS 资产使用 `DeepSeekDesktop-0.9.68-mac.dmg` 和 `DeepSeekDesktop-0.9.68-mac.zip`。
- Windows 明确标注为旧归档包，等待 v0.9.68 Windows runtime 验证。
- README、Release notes、Issue 模板和运营文档改为收集 Token共享与技能接单反馈。
- 官网和 SEO 契约保护新版定位，不再保护旧发布叙事。

完整发布说明：[docs/releases/v0.9.68.md](docs/releases/v0.9.68.md)。

## 产品截图

### 发起技能接单

<img src="assets/screenshots/desktop-conversation-home.jpg" alt="DeepSeek企业桌面版对话首页" width="900">

说明业务输出，选择模型能力，附加文件，并把任务留在同一个项目里。

### 查看执行过程

<img src="assets/screenshots/desktop-conversation-running.jpg" alt="DeepSeek企业桌面版执行过程" width="900">

任务步骤、工具动作、运行状态和人工确认边界都可见。

### 留住交付结果

<img src="assets/screenshots/desktop-conversation-result.jpg" alt="DeepSeek企业桌面版结果和文件" width="900">

结论、文件、附件和后续上下文都留在桌面工作台。

### 预览文件

<img src="assets/screenshots/desktop-file-preview.jpg" alt="DeepSeek企业桌面版文件预览" width="900">

Markdown、CSV、HTML、JSON、日志、图片、PDF 等结果可以先预览，再交给业务方。

## 反馈

最有价值的反馈是具体的：你想接什么技能、输入是什么、要交付什么文件、哪一步需要人工确认。

- [安装问题](https://github.com/guo2001china/mycodex/issues/new?template=installation_help.yml)
- [Bug 反馈](https://github.com/guo2001china/mycodex/issues/new?template=bug_report.yml)
- [功能建议](https://github.com/guo2001china/mycodex/issues/new?template=feature_request.yml)
- [模型接入或 Token共享需求](https://github.com/guo2001china/mycodex/issues/new?template=model_provider.yml)
- [社区反馈](https://github.com/guo2001china/mycodex/issues/new?template=community_feedback.yml)
- [Discussions](https://github.com/guo2001china/mycodex/discussions)

## 当前状态

DeepSeek企业桌面版当前以打包安装包形式发布，完整源码暂未在这个仓库公开。

建议先在非关键流程里试用；确认适合团队后，再放进真正需要共享模型额度和重复交付的业务流程里。
