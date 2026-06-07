<p align="center">
  <img src="https://img.shields.io/badge/GlmNote-v1.0.0-4f6ef7?style=for-the-badge" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/GLM--5.1-AI%20Powered-8A2BE2?style=for-the-badge" alt="GLM-5.1">
</p>

<p align="center">
  <a href="#-简体中文">简体中文</a> •
  <a href="#-繁體中文">繁體中文</a> •
  <a href="#-english">English</a>
</p>

---

<h1 align="center">📝 GlmNote</h1>
<p align="center"><b>基于 GLM-5.1 的智能 Markdown 知识库 · AI-Powered Markdown Knowledge Base</b></p>

---

# 🇨🇳 简体中文

## 🎉 项目介绍

**GlmNote** 是一款基于 **GLM-5.1** 大模型的智能 Markdown 知识库 Web 应用。它让你在浏览器中即可享受 **AI 增强的笔记体验**——无需安装任何软件，打开即用，所有数据安全存储在本地。

### 💡 解决的核心痛点

| 痛点 | GlmNote 的解决方案 |
|------|-------------------|
| 📝 需要好用的 Markdown 编辑器 | 实时分栏预览，所见即所得 |
| 🤖 笔记缺乏 AI 智能辅助 | 集成 GLM-5.1，可总结、解释、扩展笔记内容 |
| 🔒 数据隐私担忧 | 全部数据存储在浏览器本地，不上传任何服务器 |
| 🌐 部署复杂度高 | 纯静态 HTML，任何静态服务器即可运行 |
| 🏷️ 笔记组织困难 | 标签系统 + 全文搜索，轻松管理 |

### ✨ 与同类项目的差异化亮点

- **AI 原生集成**：原生支持 GLM-5.1 及 OpenAI 兼容 API，让 AI 成为你的知识副驾驶
- **零依赖部署**：单 HTML 文件即完整应用，无需 Node.js、无需数据库、无需构建工具
- **本地优先**：所有数据存于浏览器 localStorage，隐私安全有保障
- **极致易用**：快捷键支持、自动保存、暗色/亮色主题、一键导出 Markdown
- **多模型兼容**：支持 GLM-5.1、GPT-4o、DeepSeek 等任意 OpenAI 兼容接口

---

## ✨ 核心特性

- ⚡ **实时 Markdown 编辑** — 分栏编辑 + 实时预览，支持语法高亮和 GFM 扩展语法
- 🤖 **GLM-5.1 AI 智能助手** — 内置 AI 对话面板，可结合当前笔记进行问答、总结、解释、扩展
- 🔍 **全文搜索** — 毫秒级搜索笔记标题和内容
- 🏷️ **灵活标签系统** — 自定义标签，快速筛选和分类笔记
- 📌 **笔记置顶** — 重要笔记置顶显示，永不丢失
- 🌙 **深色/浅色主题** — 一键切换，护眼又舒适
- 📥 **一键导出** — 导出为标准 Markdown 文件
- ⌨️ **快捷键支持** — `Ctrl+N` 新建、`Ctrl+S` 保存、`Ctrl+F` 搜索、`Ctrl+I` 切换 AI 面板
- 💾 **自动保存** — 输入自动保存，再也不用担心丢失内容
- 📱 **响应式设计** — 桌面和移动设备均可流畅使用

---

## 🚀 快速开始

### 📋 环境要求

- 现代浏览器（Chrome 90+、Firefox 90+、Edge 90+、Safari 15+）
- 互联网连接（首次加载需要 CDN 资源）
- （可选）GLM-5.1 或其他大模型的 API Key

### 🛠️ 安装方式

**方式一：直接使用（推荐）**

1. 从 [Releases](https://github.com/gitstq/GlmNote/releases) 页面下载最新的 `index.html`
2. 用浏览器直接打开即可使用

**方式二：通过 HTTP 服务器运行**

```bash
# 使用 Python
cd GlmNote
python3 -m http.server 8080

# 或使用 Node.js (需要安装 http-server)
npx http-server GlmNote -p 8080
```

然后访问 `http://localhost:8080` 即可。

**方式三：使用 Docker**

```bash
docker run -d -p 8080:80 --name glmnote -v $(pwd):/usr/share/nginx/html:ro nginx:alpine
```

---

### ⚙️ 配置 AI 助手

1. 点击左下角 ⚙️ 打开设置
2. 填写 API 地址（如 GLM-5.1：`https://open.bigmodel.cn/api/paas/v4`）
3. 填写你的 API Key
4. 选择模型名称（如 `glm-5.1-flash`、`gpt-4o`、`deepseek-chat` 等）
5. 点击保存即可开始使用 AI 功能

> 💡 设置数据仅保存在浏览器本地，安全可靠

---

## 📖 详细使用指南

### 🎯 基本操作

| 操作 | 方法 |
|------|------|
| ✏️ **新建笔记** | 点击左侧 ➕ 按钮 或 `Ctrl+N` |
| 💾 **保存笔记** | 自动保存，也可按 `Ctrl+S` 手动保存 |
| 🔍 **搜索笔记** | 顶部搜索框输入关键词 或 `Ctrl+F` |
| 🏷️ **添加标签** | 点击标签栏的 `+ 标签` 按钮 |
| 📌 **置顶笔记** | 点击编辑器顶部的 📌 按钮 |
| 📥 **导出笔记** | 点击编辑器顶部的 📥 按钮 |
| 🌙 **切换主题** | 在设置中选择深色/浅色主题 |
| 🤖 **AI 助手** | 点击 🤖 按钮 或 `Ctrl+I` 打开 AI 面板 |

### 🤖 AI 助手使用场景

1. **总结笔记**：在 AI 面板输入「总结当前笔记的要点」
2. **解释代码**：选中代码片段，让 AI 解释其工作原理
3. **扩展内容**：让 AI 帮你扩写笔记的某个部分
4. **翻译文本**：让 AI 将笔记内容翻译成其他语言
5. **生成大纲**：让 AI 根据主题生成文章大纲

---

## 💡 设计思路与迭代规划

### 🎨 设计理念

GlmNote 的设计遵循三个核心原则：

1. **极简主义** — 一个 HTML 文件即可完成全部功能，拒绝臃肿
2. **隐私优先** — 数据不上传服务器，AI 交互由用户自主配置
3. **AI 原生** — 不是「笔记 + AI 插件」，而是「AI 驱动的智能知识库」

### 🏗️ 技术选型

| 技术 | 选型原因 |
|------|---------|
| **纯 HTML/CSS/JS** | 零构建步骤，开箱即用，部署成本为零 |
| **marked.js** | 业界最成熟的 Markdown 解析库，支持 GFM |
| **highlight.js** | 代码语法高亮，支持 190+ 编程语言 |
| **localStorage** | 数据本地持久化，无需后端服务 |
| **OpenAI 兼容 API** | 支持 GLM-5.1/GPT/DeepSeek 等任意大模型 |

### 🗺️ 后续迭代规划

- [ ] **WebDAV 同步** — 支持跨设备笔记同步
- [ ] **本地文件导入** — 导入本地 Markdown 文件
- [ ] **知识图谱** — 笔记间关系的可视化呈现
- [ ] **AI 自动标签** — 基于内容的智能标签推荐
- [ ] **离线 PWA** — 支持 Service Worker 离线访问
- [ ] **加密存储** — 可选的端到端加密
- [ ] **多用户协作** — 基于 WebRTC 的实时协作编辑

---

## 📦 打包与部署指南

### 部署到 GitHub Pages

```bash
# 1. Fork 本仓库
# 2. 进入仓库 Settings → Pages
# 3. Source 选择 main 分支，根目录 (/)
# 4. 等待部署完成，即可通过 https://<你的用户名>.github.io/GlmNote/ 访问
```

### 部署到 Nginx

```nginx
server {
    listen 80;
    server_name your-domain.com;
    root /var/www/GlmNote;
    index index.html;
    
    location / {
        try_files $uri $uri/ /index.html;
    }
}
```

### 兼容性

| 浏览器 | 支持情况 |
|--------|---------|
| Chrome 90+ | ✅ 完全支持 |
| Firefox 90+ | ✅ 完全支持 |
| Edge 90+ | ✅ 完全支持 |
| Safari 15+ | ✅ 完全支持 |
| IE 11 | ❌ 不支持 |

---

## 🤝 贡献指南

欢迎贡献！请遵循以下步骤：

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'feat: 添加某个很棒的功能'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 提交 Pull Request

### 提交规范

我们使用 [Conventional Commits](https://www.conventionalcommits.org/) 规范：
- `feat:` 新功能
- `fix:` 修复问题
- `docs:` 文档更新
- `style:` 代码样式调整
- `refactor:` 代码重构
- `perf:` 性能优化
- `test:` 测试相关
- `chore:` 构建/工具链

---

## 📄 开源协议

本项目采用 **MIT** 协议开源。详情请参阅 [LICENSE](LICENSE) 文件。

---

<br>

---

# 🇨🇳 繁體中文

## 🎉 專案介紹

**GlmNote** 是一款基於 **GLM-5.1** 大模型的智慧 Markdown 知識庫 Web 應用。讓你在瀏覽器中即可享受 **AI 增強的筆記體驗**——無需安裝任何軟體，打開即用，所有資料安全儲存在本地。

---

## ✨ 核心特性

- ⚡ **即時 Markdown 編輯** — 分欄編輯 + 即時預覽，支援語法高亮和 GFM 擴展語法
- 🤖 **GLM-5.1 AI 智慧助手** — 內建 AI 對話面板，可結合當前筆記進行問答、總結、解釋、擴展
- 🔍 **全文搜尋** — 毫秒級搜尋筆記標題和內容
- 🏷️ **靈活標籤系統** — 自訂標籤，快速篩選和分類筆記
- 📌 **筆記置頂** — 重要筆記置頂顯示，永不遺失
- 🌙 **深色/淺色主題** — 一鍵切換，護眼又舒適
- 📥 **一鍵匯出** — 匯出為標準 Markdown 檔案
- ⌨️ **快捷鍵支援** — `Ctrl+N` 新建、`Ctrl+S` 儲存、`Ctrl+F` 搜尋、`Ctrl+I` 切換 AI 面板
- 💾 **自動儲存** — 輸入自動儲存，再也不用擔心遺失內容
- 📱 **響應式設計** — 桌面和行動裝置均可流暢使用

---

## 🚀 快速開始

### 📋 環境要求

- 現代瀏覽器（Chrome 90+、Firefox 90+、Edge 90+、Safari 15+）
- 網際網路連線（首次載入需要 CDN 資源）
- （可選）GLM-5.1 或其他大模型的 API Key

### 🛠️ 安裝方式

**方式一：直接使用（推薦）**

從 [Releases](https://github.com/gitstq/GlmNote/releases) 頁面下載最新的 `index.html`，用瀏覽器直接開啟即可使用。

**方式二：透過 HTTP 伺服器執行**

```bash
cd GlmNote
python3 -m http.server 8080
# 或
npx http-server GlmNote -p 8080
```

訪問 `http://localhost:8080` 即可。

---

## ⚙️ 配置 AI 助手

1. 點擊左下角 ⚙️ 開啟設定
2. 填寫 API 地址（如 GLM-5.1：`https://open.bigmodel.cn/api/paas/v4`）
3. 填寫你的 API Key
4. 選擇模型名稱（如 `glm-5.1-flash`、`gpt-4o`、`deepseek-chat` 等）
5. 點擊儲存即可開始使用 AI 功能

---

## 🛠️ 部署指南

### 部署到 GitHub Pages

1. 前往倉庫 Settings → Pages
2. Source 選擇 main 分支，根目錄 (/)
3. 等待部署完成
4. 通過 `https://<你的用戶名>.github.io/GlmNote/` 訪問

---

## 📄 開源協議

本項目採用 **MIT** 協議開源。

---

<br>

---

# 🇺🇸 English

## 🎉 Introduction

**GlmNote** is an AI-powered Markdown knowledge base web application built on the **GLM-5.1** large language model. It brings **AI-enhanced note-taking** directly to your browser—no installation required, zero configuration, and all data stays securely on your device.

### 💡 Pain Points Solved

| Pain Point | GlmNote's Solution |
|------------|-------------------|
| 📝 Need a great Markdown editor | Real-time split-pane preview, WYSIWYG |
| 🤖 Notes lack AI assistance | Built-in GLM-5.1 integration for summarization, explanation, and expansion |
| 🔒 Privacy concerns | All data stored locally in browser, zero server uploads |
| 🌐 Complex deployment | Pure static HTML—works with any static server |
| 🏷️ Note organization struggles | Tag system + full-text search for easy management |

---

## ✨ Key Features

- ⚡ **Real-time Markdown Editing** — Split-pane editing with live preview, syntax highlighting, and GFM support
- 🤖 **GLM-5.1 AI Assistant** — Built-in AI chat panel that understands your current note context
- 🔍 **Full-text Search** — Lightning-fast search across note titles and content
- 🏷️ **Flexible Tag System** — Custom tags for easy filtering and categorization
- 📌 **Pin Notes** — Keep important notes always visible
- 🌙 **Dark/Light Theme** — One-click theme switching
- 📥 **One-click Export** — Export as standard Markdown files
- ⌨️ **Keyboard Shortcuts** — `Ctrl+N` new note, `Ctrl+S` save, `Ctrl+F` search, `Ctrl+I` toggle AI
- 💾 **Auto-save** — Never lose your work with automatic saving
- 📱 **Responsive Design** — Works seamlessly on desktop and mobile

---

## 🚀 Quick Start

### 📋 Requirements

- Modern browser (Chrome 90+, Firefox 90+, Edge 90+, Safari 15+)
- Internet connection (for initial CDN loading)
- (Optional) GLM-5.1 or other LLM API Key

### 🛠️ Installation

**Option 1: Direct Use (Recommended)**

Download the latest `index.html` from the [Releases](https://github.com/gitstq/GlmNote/releases) page and open it in your browser.

**Option 2: Via HTTP Server**

```bash
cd GlmNote
python3 -m http.server 8080
# or
npx http-server GlmNote -p 8080
```

Then visit `http://localhost:8080`.

---

## ⚙️ AI Setup

1. Click ⚙️ in the bottom-left to open Settings
2. Enter the API endpoint (e.g., for GLM-5.1: `https://open.bigmodel.cn/api/paas/v4`)
3. Enter your API Key
4. Select the model name (e.g., `glm-5.1-flash`, `gpt-4o`, `deepseek-chat`)
5. Click Save and start using the AI features

---

## 📖 Usage Guide

| Action | Method |
|--------|--------|
| ✏️ **New Note** | Click ➕ in sidebar or `Ctrl+N` |
| 💾 **Save** | Auto-saved, or `Ctrl+S` |
| 🔍 **Search** | Search box in sidebar or `Ctrl+F` |
| 🏷️ **Add Tag** | Click `+ 标签` in the tag bar |
| 📌 **Pin** | Click 📌 in the editor header |
| 📥 **Export** | Click 📥 in the editor header |
| 🌙 **Theme** | Settings → Theme selection |
| 🤖 **AI Panel** | Click 🤖 or `Ctrl+I` |

---

## 🚀 Deployment

### GitHub Pages

```bash
# Fork this repo
# Go to Settings → Pages
# Source: main branch, root (/)
# Access: https://<username>.github.io/GlmNote/
```

### Nginx

```nginx
server {
    listen 80;
    server_name your-domain.com;
    root /var/www/GlmNote;
    index index.html;
}
```

---

## 🗺️ Roadmap

- [ ] **WebDAV Sync** — Cross-device note synchronization
- [ ] **Local File Import** — Import existing Markdown files
- [ ] **Knowledge Graph** — Visual relationship mapping between notes
- [ ] **AI Auto-tagging** — Smart tag recommendations based on content
- [ ] **Offline PWA** — Service Worker support for offline use
- [ ] **Encrypted Storage** — Optional end-to-end encryption

---

## 🤝 Contributing

Contributions welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'feat: add some amazing feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Commit Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes
- `refactor:` Code refactoring
- `perf:` Performance improvement
- `test:` Test-related
- `chore:` Build/tooling

---

## 📄 License

This project is open-sourced under the **MIT** license. See [LICENSE](LICENSE) for details.