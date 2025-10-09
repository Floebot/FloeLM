<div align="center">

# FloeLM - Lightweight, Customizable Cross-Platform Web UI Client

Simplified Chinese · [English](/locales/README.en-US.md)

[![GitHub License](https://img.shields.io/github/license/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/blob/main/LICENSE)
[![GitHub Repo stars](https://img.shields.io/github/stars/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/network/members)
[![GitHub contributors](https://img.shields.io/github/contributors/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/graphs/contributors)
[![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/issues)

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/Floebot/FloeLM)

</div>

> [!CAUTION]
> This project is currently in preview and is not recommended for direct use in production environments. Please test it in a controlled environment and adjust configurations as needed.

FloeLM is a frontend-focused, cross-platform project designed to provide a lightweight, customizable interface for interacting with various local or remote language models (LLMs). It prioritizes interface and user experience—featuring configurable themes, conversation management, model endpoint configuration, and common session import/export capabilities—enabling rapid setup and experimentation with different model backends for conversational experiences.

![FloeLM Screenshot](/assets/screenshot.jpeg)

[Demo on GitHub.io](https://floebot.github.io/FloeLM) [Demo on Pages.dev](https://floelm.pages.dev)

## Key Features
- Pure frontend UI implementation (runs directly from static hosting).
- Configurable data and model endpoints (set API endpoints, models, and API keys in “Data Management”).
- Supports long-term sessions and one-click context clearing to preserve or reset conversation state.
- Real-time Markdown rendering with syntax highlighting for enhanced technical/development conversations.
- Support for interrupting model generation (“stop thinking”) and editing conversation messages.
- Extensive appearance/theme settings (dark/light mode, font size, compact mode, etc.).
- Import/export of conversations and settings for backup and migration.
- Design prioritizes extensibility (e.g., future integration of image recognition, visual models, or multi-model switching).

## Current Implemented / Available Features
- Left-side conversation list with common operations: search, pin, rename, delete.
- Settings panel (Appearance, Preferences, Customization, Data Management, etc.).
- Configure API Endpoints (e.g., Ollama, local/remote LLM HTTP interfaces) and model selection in Data Management.
- Session import/export and application settings import/export functionality.

## Usage Guide
- Launching the Frontend
FloeLM is a static frontend project that can be hosted using a static server (e.g., serve, http-server, nginx).<br>
Quick local testing: `npx serve` or `python -m http.server` (run in the project root directory).
- Configure Model Endpoints
After opening the application, navigate to Settings -> Data Management to set the API endpoint (e.g., your local LLM service address) and required API key (if applicable).<br>
Note: API protocols may vary across backend implementations. Adjust request formats and paths according to your LLM service.

## Configuration Considerations and Compatibility Notes
- The frontend can connect to any backend service implementing a compatible conversational API, but developers must verify that the backend's request and response formats align with FloeLM frontend expectations. If they do not, adaptation may be required in either the frontend or backend bridge layer.
- When using local model services (e.g., Ollama, llama.cpp HTTP wrappers, or other local/remote APIs), ensure the service permits cross-origin requests (CORS) or allows access via proxies.
- The current UI contains mixed Chinese and English text; contributions for complete translations are welcome.

## Contributions and Translations
- Report issues or suggest features via Issues; directly submit PRs for implementation ideas or fixes.
- If you'd like to help improve English (or other language) translations, submit a PR or indicate in an issue which sections you're willing to translate.
- Contribution workflow: Fork -> Create new branch -> Commit changes -> Open PR. Please describe the purpose and scope of changes in the PR description.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Floebot/FloeLM&type=Date)](https://www.star-history.com/#Floebot/FloeLM&Date)

## License and Disclaimer
- License: This project is licensed under the MPL-2.0. For details, refer to the LICENSE file (located in the root directory of the codebase).
- Disclaimer: Use and deployment are recommended only under conditions of compliance and security. We assume no responsibility for any illegal use of our services by users.
