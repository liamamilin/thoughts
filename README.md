# Thoughts · 个人思考档案

这是一个持续更新的**个人想法库 / 讨论库 / 结论库**。把讨论中的观察、推理、证据、分歧、暂定结论和待验证问题保存为可追溯的文章，而不是只保存一句观点。

## 入口

- 网站首页源文件：[`index.html`](index.html)
- 第一篇文章：[在中国，普通人获得可靠生活为什么这么难？](posts/2026-11-19-ordinary-life-reliability.html)
- 原始讨论纪要：[`notes/2026-11-19-ordinary-life-reliability.md`](notes/2026-11-19-ordinary-life-reliability.md)

## 目录

```text
thoughts/
├── index.html            # 首页：主题筛选与关键词搜索
├── assets/
│   ├── site.css          # 全站浅色响应式样式
│   └── site.js           # 首页本地筛选、搜索
├── posts/                # 面向阅读者的独立文章页面
├── notes/                # Markdown 源记录与历史归档
└── README.md
```

## 每次新讨论怎么入库

1. 新建 `notes/YYYY-MM-DD-short-slug.md`，包含核心结论、推理、证据状态、反证和待验证问题。
2. 创建对应的 `posts/YYYY-MM-DD-short-slug.html` 阅读页，复用 `assets/site.css`。
3. 在 `index.html` 的 `.listing` 中新增一张 `.entry` 卡片，配置分类、检索关键词、标题和标签。
4. 提交 Git，保留后续修订记录。更改结论时说明证据更新依据。

该版本采用无框架静态 HTML / CSS / JavaScript，不依赖构建工具或服务器，便于简单维护。首页搜索为本地文章索引搜索，并非全文检索。

## 发布到 GitHub Pages

仓库 Pages 发布设置**需要由仓库管理员在 GitHub 上启用**。进入 **Settings → Pages → Build and deployment**，选择 **Deploy from a branch**，并设置 **main / (root)**，保存后等待 GitHub 发布。

预期默认网址为 `https://liamamilin.github.io/thoughts/`，**只有 Pages 实际发布成功后才可确认访问**。也可本地直接打开 `index.html` 预览。

## 内容原则

- 明确区分：观察事实 / 机制推断 / 规范判断 / 待验证结论。
- 不把个别例外伪装成能推翻总体趋势的证据，也不为突出观点而杜撰比例。
- 保留讨论者真正关心的结论，不靠过多机械限定稀释它。
- 使用 [Independent Judgment Skill](https://github.com/liamamilin/skills/blob/main/skills/independent-judgment/SKILL.md) 作为论证质量规范。
