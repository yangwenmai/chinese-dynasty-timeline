# agent.md

本文件为 AI 编码助手提供项目上下文。

## 项目简介

「鼎革千年」是一个纯静态单页网站，以墨卷长轴风格展现中国上下五千年的朝代更迭与权力结构变迁。所有内容在单个 `index.html` 文件中（~2900 行，含 HTML + CSS + JS）。

## 快速启动

```bash
# 本地预览
python3 -m http.server 8000
# 访问 http://localhost:8000
```

无需安装任何依赖。

## 核心约束

- **单文件架构**：不拆分文件，HTML/CSS/JS 全部在 `index.html` 中
- **零依赖**：不引入任何外部 JS/CSS 库或图片资源
- **中文内容**：所有文案使用简体中文，引号使用「」直角引号
- **历史准确**：内容基于二十四史等正史典籍，有争议处标注「存疑」

## 编辑指南

- 新增朝代章节时，遵循 `dynasty-section > section-inner > section-divider + dynasty-header + sub-dynasty` 的 HTML 结构
- 新增颜色通过 CSS 变量定义在 `:root`，遵循 ink-/gold-/vermillion-/jade- 命名
- 新增朝代需同步更新侧边导航 `<nav class="side-nav">` 和纵览时间轴 `<section class="overview-bar">`
- 皇帝标签 class：`death`（病亡）、`murdered`（被杀）、`abdicate`（禅让/退位）、`usurp`（篡位）、`good`（治世/盛世）

## 详细规范

- 编码与内容规范：`.cursor/rules/project.mdc`
- 视觉设计体系：`.cursor/rules/design-system.mdc`
