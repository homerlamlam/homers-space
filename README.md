# 求职个人介绍网站

一个可直接部署到 GitHub Pages 的单页滚动式求职展示网站，默认中文并支持中英文切换。整体采用现代商务风 + 科技感配色，适合求职面试展示与简历配套说明。

## 本地运行

```bash
npm install
npm run build
```

构建完成后，直接打开 [docs/index.html](/C:/Users/Administrator/Documents/New%20project/docs/index.html) 或使用任意静态服务器预览 `docs/` 目录。

如需开发时实时编译样式：

```bash
npm run dev
```

## 修改入口

- 基础文案、教育经历、技能、项目、联系方式：修改 [docs/assets/app.js](/C:/Users/Administrator/Documents/New%20project/docs/assets/app.js)
- 样式主题、颜色、阴影、动画：修改 [src/styles/input.css](/C:/Users/Administrator/Documents/New%20project/src/styles/input.css)
- 页面结构：修改 [docs/index.html](/C:/Users/Administrator/Documents/New%20project/docs/index.html)

## 个人信息替换说明

1. 将 `app.js` 中所有 `【可修改占位符】` 和 `【Editable Placeholder】` 替换成你的真实信息。
2. `profileData.zh` 与 `profileData.en` 分别对应中文和英文内容。
3. 技能熟练度使用 `level` 数值控制，范围建议 `0-100`。
4. `projectsList` 中的 `link` 可替换为 GitHub、作品集或在线演示地址。
5. `contactInfo` 中的邮箱、电话、GitHub、作品集链接会自动渲染到联系方式模块。

## GitHub Pages 部署

1. 运行 `npm install`
2. 运行 `npm run build`
3. 将仓库推送到 GitHub
4. 在 GitHub Pages 设置中选择从 `main` 分支的 `/docs` 目录发布

发布后，GitHub Pages 会直接使用 `docs/` 中的静态文件。
