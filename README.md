# Mengyu Yao — Academic Homepage

这是 Mengyu Yao 的个人学术主页，基于 [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) 定制。页面采用传统学术主页的信息结构：左侧为身份与学术链接，右侧展示研究方向、论文、经历、教育和奖项。

## 本地预览

需要 Ruby、Bundler 和 Jekyll 环境：

```bash
bundle install
bash run_server.sh
```

然后访问 <http://127.0.0.1:4000>。

## 内容维护

- 主页正文：`_pages/about.md`
- 姓名、邮箱、头像与学术链接：`_config.yml`
- 顶部导航：`_data/navigation.yml`
- 样式：`assets/css/main.scss` 与 `_sass/`
- 头像：`images/profile.jpg`（由本地原图生成的网页优化版本）

`cv.tex` 是本地内容来源文件，已同时从 Git 和 Jekyll 中排除，不会进入公开仓库或生成的网站。

## GitHub Pages 部署

本站从 `main` 分支根目录部署。推送更新后，GitHub Pages 会自动使用 Jekyll 构建并发布网站。

## 致谢与许可证

本站基于 Yi Ren 的 [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io)，并保留其 MIT License。模板还借鉴了 Minimal Mistakes 与 Academic Pages；相关第三方字体和图标遵循各自许可证。
