# Personal Academic Website

一个参考简洁学术主页布局制作的个人网站模板。包括首页、论文、项目、博客、简历。使用原生 HTML / CSS / JavaScript，不需要 npm 或其他构建步骤。

## 使用方法

1. 把文件上传到名为 `你的GitHub用户名.github.io` 的 **Public** 仓库根目录（不能只上传 ZIP）。
2. 在仓库 **Settings → Pages → Build and deployment** 中选择 **Deploy from a branch**，选择 `main` / `/(root)` 并保存。
3. 打开 `https://你的GitHub用户名.github.io`。
4. 编辑 **`assets/config.js`** 修改姓名、简介、学校、研究兴趣、新闻、论文、项目、博客文章列表等。
5. 若需要头像，在 `assets/` 目录上传 `avatar.jpg`，并在 `config.js` 设置 `avatar: 'assets/avatar.jpg'`。

## 如何写博客

复制 `posts/first-post.html`，另存为如 `posts/my-new-post.html`，修改正文。注意：目前示例文章正文写在 `assets/site.js` 中 `if(page==='post')` 一段；为了不碰代码，建议每次新增博客时可以复制一个独立 HTML 页面并直接替换 `<main>` 内的正文、移除 `data-page="post"` 的自动填充逻辑。也可后续升级为 Jekyll / Markdown 博客系统。

## 文件说明

- `index.html` 首页
- `blog.html` 博客文章列表
- `publications.html` 论文
- `projects.html` 项目
- `cv.html` 简历
- `assets/config.js` **个人资料和项目数据（优先修改）**
- `assets/style.css` 网站样式
- `assets/site.js` 页面渲染逻辑

## 说明

本项目仅参考给定学术主页的公开布局与栏目组织方式；没有复制对方的个人资料、文章、照片、论文或网站源码。
