# 我的博客

这是我的个人博客，使用 Jekyll 构建并托管在 GitHub Pages 上。

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
categories: [分类]
---
```

## 部署

这个博客使用 GitHub Pages 自动部署。当你推送更改到 main 分支时，GitHub Actions 会自动构建并部署你的博客。

## 许可证

MIT License