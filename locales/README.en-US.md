# FloeLM - Lightweight, Customizable Cross-Platform Web UI Client

[简体中文](/README.md) · English

[![GitHub License](https://img.shields.io/github/license/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/blob/main/LICENSE)
[![GitHub Repo stars](https://img.shields.io/github/stars/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/network/members)
[![GitHub contributors](https://img.shields.io/github/contributors/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/graphs/contributors)
[![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/Floebot/FloeLM?style=flat-square)](https://github.com/Floebot/FloeLM/issues)

</div>

> [!CAUTION]
> This project is currently in preview and is not recommended for direct use in production environments. Please test it in a controlled environment and adjust configurations as needed.

FloeLM is a frontend-focused, cross-platform project designed to provide a lightweight, customizable interface for interacting with various local or remote language models (LLMs). It prioritizes interface and user experience—featuring configurable themes, conversation management, model endpoint configuration, and common session import/export capabilities—enabling rapid prototyping and experimentation with different model backends for conversational experiences.

![FloeLM Screenshot](./assets/screenshot.jpeg)

[Demo on GitHub.io](https://floebot.github.io/FloeLM)

## Key Features
- Pure frontend UI implementation (runs directly from static hosting).
- Configurable data and model endpoints (set API endpoints, models, and API keys in “Data Management”).
- Supports long-term sessions and one-click context clearing to preserve or reset conversation state.
- Real-time Markdown rendering with code syntax highlighting for enhanced technical/development conversations.
- Supports interrupting model generation (“stop thinking”) and editing conversation messages.
- Extensive appearance/theme settings (dark/light mode, font size, compact mode, etc.).
- Import/export conversations and settings for backup and migration.
- Designed for easy extensibility (e.g., future integration of image recognition, visual models, or multi-model switching).

## Currently Implemented / Available Features
- Left-side conversation list with common operations: search, pin, rename, delete.
- Settings panel (Appearance, Preferences, Customization).
