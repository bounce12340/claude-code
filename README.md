# Claude Code Best V3 (CCB) 🚀

<p align="center">
  <b>Claude Code CLI 工具開源實現 | Open Source Implementation of Claude Code</b>
</p>

<p align="center">
  <a href="#english">🇺🇸 English</a> • 
  <a href="#繁體中文">🇹🇼 繁體中文</a> • 
  <a href="#简体中文">🇨🇳 简体中文</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-5.0+-blue?logo=typescript" alt="TypeScript">
  <img src="https://img.shields.io/badge/Bun-1.3.11+-f5e?style=for-the-badge" alt="Bun">
  <img src="https://img.shields.io/badge/Node.js-18+-green?logo=node.js" alt="Node.js">
  <img src="https://img.shields.io/badge/version-3.0-teal" alt="Version">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

---

<a name="english"></a>
## 🇺🇸 English

> **Reverse-engineered implementation** of Anthropic's Claude Code CLI tool. Fully runnable, type-safe, enterprise-grade reliability. Compatible with both Bun and Node.js.

### ⚠️ Disclaimer

This project is for **educational and research purposes only**. All rights to Claude Code belong to Anthropic.

### ✨ Features

- **REPL Interface** — Ink-based terminal rendering (5000+ lines)
- **Multi-Provider API** — Anthropic, AWS Bedrock, Google Vertex, Azure Foundry
- **Streaming & Tool Calling** — Auto-compaction, token tracking
- **Permission System** — Plan/auto/manual modes with YOLO classifier
- **Git Worktree Support** — Isolated development environments
- **MCP Integration** — Full MCP service management

### 🚀 Quick Start

```bash
# Clone
git clone https://github.com/bounce12340/claude-code.git
cd claude-code

# Install
bun install

# Development
bun run dev  # Look for version 888
```

---

<a name="繁體中文"></a>
## 🇹🇼 繁體中文

> **Anthropic Claude Code CLI 工具的逆向工程實現**。完整可運行、類型安全、企業級可靠性。

### ⚠️ 聲明

本專案僅供**學習和研究用途**。Claude Code 的所有權利歸 Anthropic 所有。

### ✨ 特色

- **REPL 介面** — 基於 Ink 的終端渲染（5000+ 行）
- **多供應商 API** — Anthropic、AWS Bedrock、Google Vertex、Azure Foundry
- **串流與工具呼叫** — 自動壓縮、Token 追踪
- **權限系統** — Plan/auto/manual 模式
- **Git Worktree 支援** — 隔離開發環境
- **MCP 整合** — 完整 MCP 服務管理

### 🚀 快速開始

```bash
# 複製
git clone https://github.com/bounce12340/claude-code.git
cd claude-code

# 安裝
bun install

# 開發
bun run dev  # 看到版本號 888 表示成功
```

---

<a name="简体中文"></a>
## 🇨🇳 简体中文

> **Anthropic Claude Code CLI 工具的逆向工程实现**。完整可运行、类型安全、企业级可靠性。

### ⚠️ 声明

本项目仅用于**学习和研究目的**。Claude Code 的所有权利归 Anthropic 所有。

### ✨ 功能特性

- **REPL 界面** — 基于 Ink 的终端渲染（5000+ 行代码）
- **多供应商 API** — Anthropic、AWS Bedrock、Google Vertex、Azure Foundry
- **流式与工具调用** — 自动压缩、Token 追踪
- **权限系统** — Plan/auto/manual 模式
- **Git Worktree 支持** — 隔离开发环境
- **MCP 集成** — 完整 MCP 服务管理

### 🚀 快速开始

```bash
# 克隆仓库
git clone https://github.com/bounce12340/claude-code.git
cd claude-code

# 安装依赖
bun install

# 启动开发服务器
bun run dev  # 看到版本号 888 表示成功
```

### 🛠️ 技术栈

| 技术 | 说明 |
|------|------|
| **TypeScript** | 完整类型安全 |
| **Bun** | 运行时和打包工具 |
| **Ink** | 基于 React 的终端 UI |
| **Commander** | CLI 框架 |

### 📋 开发路线图

| 版本 | 状态 | 说明 |
|------|------|------|
| V1 | ✅ | 基础功能和类型检查 |
| V2 | ✅ | 完整工程化基础设施 |
| V3 | ✅ | 文档站点和完整文档 |
| V4 | 🚧 | 大量测试套件提升稳定性 |
| V5 | 📅 | 大规模重构和模块化 |

### 📦 项目结构

```
claude-code/
├── src/
│   ├── entrypoints/     # CLI 入口点
│   ├── commands/        # 斜杠命令
│   ├── tools/           # 工具实现
│   └── services/        # API、MCP、OAuth 服务
├── packages/            # Monorepo 包
│   ├── color-diff-napi/ # 终端差异高亮
│   └── computer-use/    # 计算机操作
├── build.ts            # 构建配置
└── dist/               # 构建输出
```

### 🔧 配置

在配置文件中设置你的 AI 提供商：

```json
{
  "provider": "anthropic",
  "apiKey": "your-api-key",
  "model": "claude-3-5-sonnet-20241022"
}
```

支持的提供商：Anthropic Direct、AWS Bedrock、Google Vertex、Azure Foundry。

### 📚 文档

访问我们的文档站点：https://ccb.agent-aura.top/

### 🤝 贡献

欢迎提交 PR：
- 错误修复
- 文档改进
- 测试覆盖
- 新功能

### 📄 授权

MIT License — 详见 [LICENSE](LICENSE)

### 👤 作者

**Josh** (蔡忠栩) — [@bounce12340](https://github.com/bounce12340)

---

<p align="center">
  Made with ❤️ for AI Coding Assistants<br>
  为 AI 编程助手用心打造 | 為 AI 程式編寫助手用心打造
</p>
