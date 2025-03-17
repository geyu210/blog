# 博客文章管理指南

## 功能概述
本指南详细说明如何在已部署的 Jekyll 博客中创建和管理文章，包括文章格式、元数据设置、发布流程等内容。博客已成功部署在 GitHub Pages 上，可通过 https://geyu210.github.io/blog 访问。

## 实现步骤

### 1. 创建新文章
1. 在 `_posts` 目录下创建新的 Markdown 文件
2. 文件名格式：`YYYY-MM-DD-title.md`（如 `2024-03-17-hello-world.md`）
3. 添加必要的 front matter

### 2. 文章 Front Matter 配置
```yaml
---
layout: post
title: "文章标题"
date: YYYY-MM-DD HH:MM:SS +0800
categories: [分类1, 分类2]
tags: [标签1, 标签2]
---
```

### 3. 文章内容编写
1. 使用 Markdown 语法
2. 支持代码高亮
3. 可以插入图片和链接

### 4. 发布流程
1. 将新文章提交到 Git 仓库
2. 推送到 GitHub `main` 分支
3. GitHub Actions 自动构建并部署
4. 几分钟后可在博客网站上查看新文章

## 关键决策点
| 决策点 | 选择方案 | 决策理由 | 替代方案 |
|-------|---------|---------|---------|
| 文章格式 | Markdown | 易读易写，广泛支持 | HTML |
| 图片存储 | 本地存储 | 便于管理，加载快 | 外部图床 |
| 分类方式 | 多级分类 | 内容组织清晰 | 标签系统 |
| 部署方式 | GitHub Actions | 自动化，稳定可靠 | 手动部署 |

## 注意事项
- 确保文件名和 front matter 中的日期一致
- 图片路径使用相对路径，放在 `assets/images` 目录
- 使用 GitHub 官方支持的 Markdown 和 Jekyll 插件功能
- 大型资源文件考虑使用外部存储

## 测试策略
- 提交前在本地预览（可选）
- 提交后检查 GitHub Actions 构建状态
- 访问博客站点确认新文章显示正常
- 检查图片和链接是否可用

## 示例文章
```markdown
---
layout: post
title: "我的第一篇博客文章"
date: 2024-03-17 12:00:00 +0800
categories: [技术, 生活]
tags: [Jekyll, 博客]
---

## 引言
这是我的第一篇博客文章，在这里我将分享我的想法和经验。

## 正文
这里是文章的主要内容...

### 代码示例
```python
def hello_world():
    print("Hello, World!")
```

## 总结
感谢阅读！
```

## 常见问题解决方案

### 1. 文章不显示
- 检查文件名格式是否正确
- 验证 front matter 格式是否有误
- 确认 GitHub Actions 构建是否成功
- 确认文件编码为 UTF-8

### 2. 图片显示问题
- 检查图片路径是否正确
- 确认图片已上传到正确位置
- 验证图片格式是否受支持

### 3. 格式问题
- 使用标准 Markdown 语法
- 参考 GitHub Flavored Markdown 规范
- 使用 GitHub 官方支持的 Jekyll 功能

## 最佳实践
1. 定期更新博客内容
2. 按主题和类别组织文章
3. 使用清晰的标题和描述
4. 添加适当的分类和标签
5. 包含相关图片和代码示例（适当情况）
6. 保持内容原创性和价值
7. 定期检查和修复失效链接 