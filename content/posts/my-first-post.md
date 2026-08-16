---
title: "我的第一篇博文"
date: 2026-08-16
draft: false
tags: ["博客搭建", "Hugo"]
categories: ["随笔"]
summary: "博客正式开通：Hugo + PaperMod + GitHub Pages，push 即发布。"
---

## 你好，世界

这里是 AvonLyn 的博客，终于搭好了。

## 这个博客是怎么搭的

- **静态站点生成器**：Hugo（extended 版）
- **主题**：PaperMod
- **托管**：GitHub Pages（`AvonLyn.github.io`）
- **部署**：GitHub Actions，push 到 `main` 分支自动构建发布
- **评论**：giscus（基于 GitHub Discussions）

## 写作方式

在 `content/posts/` 下新建 Markdown 文件：

```bash
hugo new content content/posts/新文章.md
```

写完 push 到 `main`，几分钟后线上可见。

## 接下来

慢慢填坑。
