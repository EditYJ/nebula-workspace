<div align="center">

<img src="public/logo.svg" alt="Nebula Logo" width="120" />

# Nebula

**基于 Tauri v2 构建的现代 VDI 管理看板与 AI 助手**

[![Tauri](https://img.shields.io/badge/Tauri-v2-24C8DB?style=flat&logo=tauri&logoColor=white)](https://tauri.app/)
[![React](https://img.shields.io/badge/React-v19-61DAFB?style=flat&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-38B2AC?style=flat&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

[English](./README.md) | [简体中文](./README_zh-CN.md)

</div>

---

### 简介
**Nebula** 是一款基于 **Tauri v2** 和 **React** 构建的高性能桌面应用程序。它旨在提供流畅的虚拟桌面基础架构 (VDI) 管理体验，并集成了由 **Google Gemini** 驱动的 AI 智能助手。

### 📸 预览
<div align="center">
  <img src="docs/login_dark.png" alt="仪表盘预览" width="800" />
  <p><em>登录页与接入网关</em></p>
  
  <br />
  
  <img src="docs/home_dark.png" alt="AI 助手预览" width="800" />
  <p><em>主仪表盘与数据分析</em></p>
</div>

### ✨ 主要特性
- **🤖 AI 智能助手**: 集成 `@google/genai`，提供智能对话辅助，帮助用户解决问题和执行操作。
- **🖥️ VDI 查看器**: 专门的虚拟桌面查看与管理界面。
- **📊 数据看板**: 使用 `recharts` 实现的实时数据可视化仪表盘。
- **🎨 现代 UI/UX**: 基于 **Tailwind CSS v4** 和 **Lucide React** 图标库构建的现代化响应式界面。
- **🌍 多语言支持**: 内置多语言切换支持 (`LanguageContext`)。
- **⚙️ 个性化设置**: 完善的用户资料管理与系统设置功能。

### 🛠️ 技术栈
- **核心框架**: [Tauri v2](https://v2.tauri.app/) (Rust + Webview)
- **前端框架**: React 19, TypeScript, Vite 7
- **样式方案**: Tailwind CSS v4
- **状态管理**: React Context API
- **AI 集成**: Google Gemini API
- **图表库**: Recharts

### 🚀 快速开始

#### 环境要求
- **Node.js** (推荐最新 LTS 版本)
- **pnpm** (包管理器)
- **Rust** (Tauri 开发必需) - [安装 Rust](https://www.rust-lang.org/tools/install)

#### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/jience/nebula-workspace.git
   cd nebula
   ```

2. **安装依赖**
   ```bash
   pnpm install
   ```

3. **开发模式**
   启动前端和 Tauri 后端进入开发模式：
   ```bash
   pnpm tauri dev
   ```

4. **生产构建**
   构建优化后的生产版本/安装包：
   ```bash
   pnpm tauri build
   ```

### 📂 项目结构
```text
nebula/
├── src/
│   ├── components/      # UI 组件 (仪表盘, 聊天, VDI 查看器)
│   ├── contexts/        # 全局状态 (主题, 语言)
│   ├── services/        # API 服务 (Gemini AI)
│   └── styles/          # Tailwind 配置
├── src-tauri/           # Rust 后端 (Tauri 配置)
└── vite.config.ts       # Vite 配置
```

### 🤝 贡献者
感谢所有为该项目做出贡献的人！
<a href="https://github.com/jience/nebula-workspace/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=jience/nebula-workspace" />
  <img src="https://contrib.rocks/image?repo=EditYJ/nebula-workspace" />
</a>

### 📄 开源协议
本项目采用 [MIT License](LICENSE) 协议开源 - 详情请参阅文件。

