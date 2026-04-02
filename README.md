# Claude Code Best V3 (CCB) 🚀

<p align="center">
  <strong>Claude Code CLI 工具開源實現 — 類型安全、工程化完備、企業級可靠性</strong>
</p>

<p align="center">
  <strong>English</strong> | <strong>繁體中文</strong>
</p>

<p align="center">
  <a href="https://github.com/claude-code-best/claude-code"><img src="https://img.shields.io/badge/upstream-claude--code--best-purple?style=for-the-badge" alt="Upstream"></a>
  <a href="#quick-start"><img src="https://img.shields.io/badge/Quick_Start-3_min-blue?style=for-the-badge" alt="Quick Start"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="License"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-5.0+-blue?logo=typescript" alt="TypeScript">
  <img src="https://img.shields.io/badge/Bun-1.3.11+-f5e?style=for-the-badge" alt="Bun">
  <img src="https://img.shields.io/badge/Node.js-18+-green?logo=node.js" alt="Node.js">
  <img src="https://img.shields.io/badge/version-3.0-teal" alt="Version">
</p>

---

## 🇬🇧 English

> **Reverse-engineered implementation** of Anthropic's Claude Code CLI tool. Fully runnable, type-safe, enterprise-grade reliability. Compatible with both Bun and Node.js.

### ⚠️ Disclaimer

This project is for **educational and research purposes only**. All rights to Claude Code belong to Anthropic.

### 🚀 Quick Start

#### Prerequisites

- **Bun** >= 1.3.11 (highly recommended)
- Node.js 18+ (optional, for Node builds)

#### Installation

```bash
# Clone the repository
git clone https://github.com/bounce12340/claude-code.git
cd claude-code

# Install dependencies
bun install
```

#### Development

```bash
# Start development server (look for version 888 in output)
bun run dev

# Build for production
bun run build
```

The build uses code splitting (approximately 450 chunks) and outputs to `dist/` directory. Both Bun and Node.js can run the built artifacts.

### 📋 Roadmap

| Version | Status | Description |
|---------|--------|-------------|
| V1 | ✅ | Basic functionality and type checking |
| V2 | ✅ | Complete engineering infrastructure |
| V3 | ✅ | Documentation site and comprehensive docs |
| V4 | 🚧 | Extensive test suite for stability |
| V5 | 📅 | Major refactoring and modularization |

### ✨ Features

- **REPL Interface** — Ink-based terminal rendering (5000+ lines)
- **Multi-Provider API** — Anthropic, AWS Bedrock, Google Vertex, Azure Foundry
- **Streaming & Tool Calling** — Auto-compaction, token tracking
- **Permission System** — Plan/auto/manual modes with YOLO classifier
- **Git Worktree Support** — Isolated development environments
- **MCP Integration** — Full MCP service management
- **Plugin System** — Extensible plugin architecture

### 🛠️ Tech Stack

- **TypeScript** — Full type safety
- **Bun** — Runtime and bundler
- **Ink** — React-based terminal UI
- **Commander** — CLI framework

### 📦 Project Structure

```
claude-code/
├── src/
│   ├── entrypoints/        # CLI entry points
│   ├── commands/            # Slash commands
│   ├── tools/               # Tool implementations
│   ├── services/            # API, MCP, OAuth services
│   └── types/               # Type definitions
├── packages/                # Monorepo packages
│   ├── color-diff-napi/     # Terminal diff highlighting
│   ├── audio-capture-napi/  # Audio recording
│   └── image-processor-napi/# Image processing
├── scripts/                 # Build scripts
├── build.ts                 # Build configuration
└── dist/                    # Build output
```

### 🔧 Configuration

Configure your AI provider in settings:

```json
{
  "provider": "anthropic",
  "apiKey": "your-api-key",
  "model": "claude-3-5-sonnet-20241022"
}
```

Supported providers: Anthropic Direct, AWS Bedrock, Google Vertex, Azure Foundry.

### 📚 Documentation

Visit our documentation site: https://ccb.agent-aura.top/

### 🤝 Contributing

Contributions are welcome! Please submit PRs for:
- Bug fixes
- Documentation improvements
- Test coverage
- New features

### 📄 License

MIT License — See [LICENSE](LICENSE) for details.

---

## 🇹🇼 繁體中文

> **Anthropic Claude Code CLI 工具的逆向工程實現**。完整可運行、類型安全、企業級可靠性。支援 Bun 和 Node.js 雙運行。

### ⚠️ 聲明

本專案僅供**學習和研究用途**。Claude Code 的所有權利歸 Anthropic 所有。

### 🚀 快速開始

#### 環境要求

- **Bun** >= 1.3.11（強烈建議）
- Node.js 18+（選擇性，供 Node 構建使用）

#### 安裝

```bash
# 複製倉庫
git clone https://github.com/bounce12340/claude-code.git
cd claude-code

# 安裝依賴
bun install
```

#### 開發

```bash
# 啟動開發伺服器（看到版本號 888 表示成功）
bun run dev

# 構建生產版本
bun run build
```

構建採用程式碼分割（約 450 個區塊），輸出到 `dist/` 目錄。Bun 和 Node.js 都可以運行構建產物。

### 📋 開發路線圖

| 版本 | 狀態 | 說明 |
|------|------|------|
| V1 | ✅ | 基礎功能和類型檢查 |
| V2 | ✅ | 完整工程化基礎設施 |
| V3 | ✅ | 文件網站和完整文件 |
| V4 | 🚧 | 大量測試套件提升穩定性 |
| V5 | 📅 | 大規模重構和模組化 |

### ✨ 功能特色

- **REPL 介面** — 基於 Ink 的終端渲染（5000+ 行程式碼）
- **多供應商 API** — Anthropic、AWS Bedrock、Google Vertex、Azure Foundry
- **串流和工具呼叫** — 自動壓縮、Token 追踪
- **權限系統** — Plan/auto/manual 模式，含 YOLO 分類器
- **Git Worktree 支援** — 隔離開發環境
- **MCP 整合** — 完整 MCP 服務管理
- **插件系統** — 可擴展插件架構

### 🛠️ 技術棧

- **TypeScript** — 完整類型安全
- **Bun** — 執行時期和打包工具
- **Ink** — 基於 React 的終端 UI
- **Commander** — CLI 框架

### 📦 專案結構

```
claude-code/
├── src/
│   ├── entrypoints/        # CLI 入口點
│   ├── commands/            # 斜線命令
│   ├── tools/               # 工具實作
│   ├── services/            # API、MCP、OAuth 服務
│   └── types/               # 類型定義
├── packages/                # Monorepo 套件
│   ├── color-diff-napi/     # 終端差異高亮
│   ├── audio-capture-napi/  # 音訊錄製
│   └── image-processor-napi/# 圖片處理
├── scripts/                 # 構建腳本
├── build.ts                 # 構建設定
└── dist/                    # 構建輸出
```

### 🔧 設定

在設定中配置你的 AI 供應商：

```json
{
  "provider": "anthropic",
  "apiKey": "your-api-key",
  "model": "claude-3-5-sonnet-20241022"
}
```

支援的供應商：Anthropic Direct、AWS Bedrock、Google Vertex、Azure Foundry。

### 📚 文件

訪問我們的文件網站：https://ccb.agent-aura.top/

### 🤝 貢獻

歡迎貢獻！請提交 PR：
- 錯誤修復
- 文件改進
- 測試覆蓋
- 新功能

### 📄 授權

MIT 授權 — 詳見 [LICENSE](LICENSE)。

---

## 📊 能力清單 / Capability Matrix

### 核心系統 / Core Systems

| 能力 | 狀態 | 說明 |
|------|------|------|
| REPL 交互介面 | ✅ | Ink 終端渲染，主螢幕 5000+ 行 |
| API 通信 — Anthropic | ✅ | 支援 API Key + OAuth |
| API 通信 — AWS Bedrock | ✅ | 支援憑證刷新、Bearer Token |
| API 通信 — Google Vertex | ✅ | 支援 GCP 憑證刷新 |
| API 通信 — Azure Foundry | ✅ | 支援 API Key + Azure AD |
| 串流對話與工具呼叫 | ✅ | 自動壓縮、Token 追踪 |
| 會話引擎 | ✅ | 管理對話狀態與歸因 |
| 上下文構建 | ✅ | git status、CLAUDE.md、memory |
| 權限系統 | ✅ | Plan/auto/manual 模式 |
| 會話恢復 | ✅ | ResumeConversation 螢幕 |
| Doctor 診斷 | ✅ | 版本、API、插件、沙箱檢查 |
| 自動壓縮 | ✅ | auto-compact、micro-compact |

### 工具 / Tools

| 工具 | 狀態 | 說明 |
|------|------|------|
| BashTool | ✅ | Shell 執行、沙箱、權限檢查 |
| FileReadTool | ✅ | 檔案/PDF/圖片/Notebook 讀取 |
| FileEditTool | ✅ | 字串替換式編輯 + diff 追踪 |
| FileWriteTool | ✅ | 檔案建立/覆寫 + diff 生成 |
| WebFetchTool | ✅ | URL 抓取 → Markdown |
| WebSearchTool | ✅ | 網頁搜尋 + 域名篩選 |
| AgentTool | ✅ | 子代理派生 |
| SkillTool | ✅ | 斜線命令 / Skill 呼叫 |
| MCP 工具 | ✅ | MCP 資源列表、讀取 |
| CronCreateTool | ✅ | 定時任務建立 |
| Git Worktree | ✅ | 進入/退出 Git Worktree |

### 斜線命令 / Slash Commands

| 命令 | 狀態 | 說明 |
|------|------|------|
| /add-dir | ✅ | 新增目錄 |
| /config | ✅ | 設定管理 |
| /doctor | ✅ | 健康檢查 |
| /help | ✅ | 幫助 |
| /login / /logout | ✅ | 登入/登出 |
| /memory | ✅ | Memory / CLAUDE.md 管理 |
| /mcp | ✅ | MCP 服務管理 |
| /permissions | ✅ | 權限管理 |
| /plan | ✅ | 計劃模式 |
| /skills | ✅ | Skill 管理 |
| /tasks | ✅ | 任務管理 |
| /usage | ✅ | 用量資訊 |
| /upgrade | ✅ | 升級 CLI |

---

## 🏗️ 專案結構詳解 / Project Structure Deep Dive

```
claude-code/
├── src/
│   ├── entrypoints/
│   │   ├── cli.tsx          # 入口檔案（含 MACRO/feature polyfill）
│   │   └── sdk/             # SDK 子模組 stub
│   ├── main.tsx             # 主 CLI 邏輯（Commander 定義）
│   ├── commands/            # 斜線命令實作
│   ├── tools/               # 工具實作
│   ├── services/            # 服務層
│   │   ├── api/            # API 客戶端
│   │   ├── mcp/            # MCP 服務
│   │   ├── oauth/          # OAuth 流程
│   │   ├── plugins/        # 插件系統
│   │   └── compact/        # 壓縮服務
│   └── types/
│       ├── global.d.ts     # 全域變數/巨集聲明
│       └── internal-modules.d.ts  # 內部 npm 套件類型聲明
├── packages/                # Monorepo workspace 套件
│   ├── color-diff-napi/     # 完整實作（終端 color diff）
│   ├── audio-capture-napi/  # 音訊錄製
│   ├── image-processor-napi/# 圖片處理
│   ├── modifiers-napi/      # 修飾鍵檢測
│   └── @ant/              # Anthropic 內部套件
│       ├── computer-use-mcp/
│       ├── computer-use-input/
│       └── computer-use-swift/
├── scripts/                 # 自動化 stub 生成腳本
├── build.ts                # 構建腳本（Bun.build + code splitting）
├── dist/                   # 構建輸出（入口 cli.js + ~450 chunk 檔案）
└── package.json            # Bun workspaces monorepo 設定
```

---

## 🔬 Feature Flags 詳解

原版 Claude Code 透過 `bun:bundle` 的 `feature()` 在構建時注入 feature flag。本專案中 `feature()` 被 polyfill 為始終回傳 `false`，因此以下功能目前關閉：

### 自主 Agent
- `KAIROS` — 長期運行的自主 Agent 模式
- `PROACTIVE` — 主動模式，Agent 主動執行任務
- `BUDDY` — Buddy 配對編輯功能

### 遠端/分散式
- `BRIDGE_MODE` — 遠端控制橋接
- `DAEMON` — 守護程序模式
- `SSH_REMOTE` — SSH 遠端連線

### 增強工具
- `VOICE_MODE` — 語音輸入輸出
- `WEB_BROWSER_TOOL` — 網頁瀏覽器工具
- `WORKFLOW_SCRIPTS` — 工作流腳本

---

## 📈 Star History

> 開源後記錄：
- 48 小時：突破 7k Star
- 24 小時：突破 6k Star
- 15 小時：突破 3k Star
- 12 小時：突破 1k Star

---

<div align="center">

**Claude Code Best** — *開源實現，學習研究*

</div>
