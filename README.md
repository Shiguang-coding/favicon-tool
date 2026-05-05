# 🎯 Favicon 工坊 - 双模式网站图标下载器

一个功能强大的在线工具，用于从任何网站快速提取并下载 Favicon（网站图标）。支持 PNG、JPEG、WebP、ICO 等多种格式，并提供快速和增强两种工作模式。

[![在线使用](https://img.shields.io/badge/在线使用-点击体验-brightgreen)](https://yourusername.github.io/favicon-tool)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/yourusername/favicon-tool/pulls)

## ✨ 特性

### 双模式设计

| 特性          | ⚡ 快速模式 (V1)   | 🚀 增强模式 (V2)         |
| ------------- | ----------------- | ----------------------- |
| **获取速度**  | 极快，直接请求    | 稍慢，通过代理          |
| **支持格式**  | PNG / JPEG / WebP | PNG / JPEG / WebP / ICO |
| **尺寸调整**  | ❌ 保持原图尺寸    | ✅ 16-512px 自由调整     |
| **CORS 限制** | 无                | 已通过代理解决          |
| **适用场景**  | 快速下载原图      | 需要特定尺寸或 ICO 格式 |

### 核心功能

- ✅ 从任意网站提取 Favicon
- ✅ 实时预览图标
- ✅ 多格式下载（PNG、JPEG、WebP、ICO）
- ✅ 尺寸自由调整（V2 模式：16px - 512px）
- ✅ 智能多源获取策略
- ✅ 完全前端实现，隐私安全
- ✅ 响应式设计，支持移动端

## 🚀 在线使用

访问：[https://favicontool.shiguang666.eu.org](https://favicontool.shiguang666.eu.org)

或者下载 HTML 文件到本地直接打开使用。

## 📖 使用指南

### 快速开始

1. **输入网址** - 支持 `github.com` 或 `https://apple.com` 格式
2. **选择模式** - 点击切换快速模式或增强模式
3. **获取图标** - 点击"获取图标"按钮
4. **选择格式** - PNG / JPEG / WebP / ICO
5. **调整尺寸**（增强模式）- 使用滑块或快捷按钮
6. **下载** - 点击下载按钮保存图标

### 模式选择建议

- **快速模式**：适合大多数网站，速度最快，支持主流格式
- **增强模式**：当需要特定尺寸或 ICO 格式时使用，通过代理解决跨域问题

## 🛠️ 技术实现

### 数据源（图标服务）

工具使用以下服务获取网站图标：

| 服务                   | 网址                                                         | 说明                      | 使用模式 |
| ---------------------- | ------------------------------------------------------------ | ------------------------- | -------- |
| **Google S2 Favicons** | [https://www.google.com/s2/favicons](https://www.google.com/s2/favicons) | Google 提供的稳定图标服务 | V1 / V2  |
| **Icon Horse**         | [https://icon.horse](https://icon.horse)                     | 高质量图标服务            | V1 / V2  |
| **Favicon Kit**        | [https://faviconkit.com](https://faviconkit.com)             | 备选图标服务              | V1       |

### 代理服务

增强模式使用以下代理服务解决跨域资源共享（CORS）限制：

| 服务               | 网址                                             | 说明                       |
| ------------------ | ------------------------------------------------ | -------------------------- |
| **allorigins.win** | [https://allorigins.win](https://allorigins.win) | 免费、稳定的 CORS 代理服务 |

### 技术栈

- 原生 HTML5 / CSS3 / JavaScript
- Canvas API（图像处理）
- File API / Blob（文件下载）
- Fetch API（网络请求）

## 🔧 本地运行

由于工具完全前端实现，无需任何服务器环境：

```bash
# 方法1：直接双击打开
open index.html
# 方法2：使用本地服务器（推荐）
npx serve .
# 或
python -m http.server 8000
```

## ☁️ 部署到 Vercel

### 准备工作

1. 注册 [Vercel](https://vercel.com/) 账号（支持 GitHub 登录）
2. 将本项目代码推送到 GitHub 仓库

### 部署步骤

#### 方法一：一键部署（推荐）

点击下方按钮，自动完成部署：

https://vercel.com/button

#### 方法二：通过 Vercel CLI 部署

bash

```
# 安装 Vercel CLI
npm i -g vercel

# 进入项目目录
cd favicon-tool

# 部署
vercel

# 按照提示完成部署
```

#### 方法三：连接 GitHub 自动部署

1. 登录 Vercel 控制台
2. 点击 "Add New" → "Project"
3. 选择包含本项目的 GitHub 仓库
4. 点击 "Deploy"

部署完成后，Vercel 会自动分配一个 `*.vercel.app` 域名，您也可以在设置中绑定自定义域名。

## 🙏 特别鸣谢

感谢以下服务和项目：

### 图标服务
- [Google S2 Favicons](https://www.google.com/s2/favicons) - Google 图标服务
- [Icon Horse](https://icon.horse) - 高质量图标服务
- [favicon.im](https://favicon.im) - UI 设计灵感来源

## ⭐ 支持项目

如果这个项目对您有帮助，请给一个 Star ⭐，这是对我最大的鼓励！

## 🔒 隐私说明

- 本工具**完全前端实现**，不收集任何用户数据
- 所有图片处理均在本地浏览器完成
- 不向任何服务器上传您的数据



