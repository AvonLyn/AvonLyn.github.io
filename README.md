# AvonLyn 的博客

基于 **Hugo + PaperMod** 的个人博客，托管在 GitHub Pages：

**线上地址**：https://avonlyn.github.io

## 常用命令

```bash
# 新建文章（写完后把 draft: true 改成 false）
hugo new content content/posts/文章名.md

# 本地预览（含草稿）
hugo server -D
# 打开 http://localhost:1313

# 本地构建
hugo --gc --minify
```

## 发布流程

push 到 `main` 分支即可，GitHub Actions（`.github/workflows/hugo.yaml`）会自动构建并部署，几分钟后线上更新。

```bash
git add -A
git commit -m "Add new post"
git push
```

## 目录结构

- `content/posts/` — 博文
- `content/archives.md` / `search.md` / `about.md` — 归档 / 搜索 / 关于页面
- `layouts/_partials/comments.html` — giscus 评论配置
- `hugo.yaml` — 站点配置（菜单、Profile 模式、搜索、社交图标等）
- `themes/PaperMod/` — 主题（git 子模块，不要直接改）

## 小备忘

- 头像：图片放 `assets/images/`，然后在 `hugo.yaml` 的 `profileMode` 里设置 `imageUrl`
- 克隆本仓库需带子模块：`git clone --recurse-submodules`
