<div align="center">

# FloeLM - 轻量可定制的跨平台 Web UI 客户端

简体中文 · [English](./locales/README.en-US.md)

[![GitHub License](https://img.shields.io/github/license/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/blob/main/LICENSE)
[![GitHub Repo stars](https://img.shields.io/github/stars/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/network/members)
[![GitHub contributors](https://img.shields.io/github/contributors/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/graphs/contributors)
[![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/issues)

</div>

> [!CAUTION]
> 本项目目前处于预览阶段，不建议直接用于生产环境，请在受控环境中测试并根据需要调整配置。

FloeLM 是一个以前端为主的跨平台项目，目标是为各种本地或远端语言模型（LLM）提供一个轻量、可定制的交互界面。它专注于界面与用户体验——拥有可配置的主题、对话管理、模型端点配置以及常用的会话导入导出功能，便于快速搭建与试验不同模型后端的对话体验。

![FloeLM Screenshot](./assets/screenshot.jpeg)

[Demo on GitHub.io](https://floebot.github.io/FloeLM)

## 主要特点
- 纯前端实现的 UI（静态托管即可运行前端界面）。
- 可配置的数据与模型端点（在“Data Management”中配置 API endpoint、模型及 API key）。
- 支持长会话与一键清除上下文，便于保持或重置对话状态。
- 实时 Markdown 渲染与代码语法高亮，提升开发/技术类对话体验。
- 支持中断模型生成（stop thinking）与对话消息编辑。
- 丰富的外观/主题设置（暗色/亮色、字体大小、紧凑模式等）。
- 会话与设置的导入/导出，便于备份与迁移。
- 设计上便于扩展（例如后续接入图片识别、视觉模型或多模型切换）。

## 当前已实现 / 可用的功能
- 左侧会话列表与搜索、置顶、重命名、删除等常见操作。
- 设置面板（Appearance、Preferences、Customization、Data Management 等）。
- 在 Data Management 中配置 API Endpoint（例如 Ollama、本地或远端 LLM HTTP 接口）与模型选择。
- 会话导入/导出以及应用设置的导入/导出功能。

## 使用指南
- 获取代码
克隆仓库或下载源码文件。
- 启动前端
FloeLM 是静态前端项目，使用静态服务器（如 serve、http-server、nginx 等）托管即可.
本地快速测试：`npx serve` 或 `python -m http.server`（在项目根目录运行）。
- 配置模型端点
打开应用后进入 Settings -> Data Management，设置 API endpoint（例如本地的 LLM 服务地址）以及需要的 API key（如适用）。
说明：不同后端实现的 API 协议可能不同，请根据所用 LLM 服务调整请求格式与路径。

## 配置要点与兼容性提示
- 前端可连接任意实现了兼容对话 API 的后端服务，但需要开发者确认后端的请求与返回格式是否与 FloeLM 前端预期一致；如不一致，可能需要在前端或后端桥接层进行适配。
- 如果使用本地模型服务（如 Ollama、llama.cpp HTTP 封装或其它本地/远端 API），请确保服务允许跨域（CORS）或通过代理访问。
- 目前 UI 有中英文混合的情况，欢迎贡献完整翻译。

## 贡献与翻译
- 欢迎通过 Issues 报告问题或提出功能建议；如果你有实现想法或修复也欢迎直接提交 PR。
- 如果你愿意帮助完善英文（或其他语言）翻译，请提交 PR 或在 issue 中标明你愿意翻译的部分。
- 贡献流程：Fork -> 新分支 -> 提交 -> 发起 PR。请在 PR 描述中说明变更目的与影响范围。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Floebot/FloeLM&type=Date)](https://www.star-history.com/#Floebot/FloeLM&Date)

## 许可与声明
- 许可证：本软件采用MPL-2.0许可证授权，详情请参阅 LICENSE 文件（位于代码库根目录下）。
- 免责声明：建议在合规与安全的前提下使用与部署，对于用户对我们服务的任何非法使用，我们概不负责。
