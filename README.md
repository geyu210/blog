# 我的博客

这是我的个人博客，使用 Jekyll 构建并托管在 GitHub Pages 上。博客已成功部署，可通过 https://geyu210.github.io/blog 访问。

## 博客特点

- 简洁美观的 Minima 主题
- 支持 Markdown 格式的文章
- 文章分类和标签功能
- 自动构建和部署

## 本地开发

要在本地运行这个博客，你需要：

1. 安装 Ruby 和 Bundler
2. 安装依赖：
   ```bash
   bundle install
   ```
3. 启动本地服务器：
   ```bash
   bundle exec jekyll serve
   ```
4. 访问 http://localhost:4000 查看博客

## 写作新文章

要创建新的博客文章，在 `_posts` 目录下创建一个新的 Markdown 文件，文件名格式为：`YYYY-MM-DD-title.md`。

文章开头需要包含以下 front matter：

```yaml
---
layout: post
title: "文章标题"
date: YYYY-MM-DD HH:MM:SS +0800
categories: [分类1, 分类2]
tags: [标签1, 标签2]
---
```

## 部署

这个博客使用 GitHub Pages 自动部署。当你推送更改到 main 分支时，GitHub Actions 会自动构建并部署你的博客。部署通常在几分钟内完成。

## 项目文档

- [AI项目参考文档](PROJECT_ARCHITECTURE.md) - 为AI助手提供的详细项目结构、数据流和操作指南
- [博客文章管理指南](BLOG_POST_GUIDE.md) - 如何创建和管理博客文章

## 许可证

MIT License