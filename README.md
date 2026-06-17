# <img src="brand/icon-light.svg" width="32" height="32" alt="Favicon 工坊 Logo"> Favicon 工坊

一个纯前端、隐私安全的在线工具，用于从任意网站快速提取并下载 Favicon。支持多源切换、尺寸调整、多格式导出。

[![在线使用](https://img.shields.io/badge/在线使用-点击体验-brightgreen)](https://favicon.shiguang666.eu.org)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

## ✨ 特性

- **多源智能获取** - 自动轮询多个图标服务，保证高成功率
- **手动换源** - 一键切换数据源，透明显示当前源及进度
- **尺寸调整** - 16px - 512px 自由缩放，支持快捷预设
- **多格式导出** - PNG / JPG / WebP / ICO
- **多主题** - 内置 8 套主题（暗夜霓虹、复古街机、日式侘寂等）
- **隐私安全** - 所有处理在本地浏览器完成，不上传任何数据

## 🚀 在线使用

![image-20260614140902908](https://img.shiguang666.eu.org/file/1781417348268_20260614140903862.webp)

访问：[https://favicon.shiguang666.eu.org](https://favicon.shiguang666.eu.org)

或直接下载 `index.html` 在浏览器中打开。

## 📖 使用指南

1. **输入网址** - 支持 `github.com` 或 `https://apple.com` 格式
2. **提取图标** - 自动从最优源获取
3. **换源** - 不满意可手动切换其他数据源
4. **调整尺寸** - 拖动滑块或点击预设尺寸
5. **选择格式** - PNG / JPG / WebP / ICO
6. **下载** - 一键保存

## 🛠️ 数据源

| 服务 | 说明 |
| --- | --- |
| **[icon.horse](https://icon.horse)** | 高质量图标服务，默认首选 |
| **[favicon.so](https://favicon.so)** | 备选图标服务 |
| **favicon.ico** | 直接请求目标网站的 /favicon.ico |

## 🎨 主题

支持 8 套主题：经典街机、暗夜霓虹、复古街机、日式侘寂、赛博终端、极光渐变、瑞士极简、温暖工坊。

## 🖥️ 本地运行

```bash
# 直接双击 index.html 打开
# 或使用本地服务器
npx serve .
```

## 📦 部署

支持一键部署到 Vercel：

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FShiguang-coding%2Ffavicon-tool)

## 🔒 隐私说明

- 完全前端实现，无后端服务
- 图片处理均在本地浏览器完成
- 不收集任何用户数据
