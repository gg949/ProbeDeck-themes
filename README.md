# ProbeDeck-themes

ProbeDeck 主题商店目录。面板（v2.12.5+）从本仓库的 `themes.json` 拉取商店列表。

- 现有 7 个主题（Emerald / Pulse / LuminaPlus / Horizon / Junimo / Shadcn / Glassmorphism）顺序固定，**不要改它们的 `id` / 顺序 / `url`**。
- 内置 Mikus 写在面板里，不进本仓库。
- 新第三方主题**追加到数组末尾**，不要插到中间。
- 加主题 = 改本仓库并 push。已升级到 v2.12.5+ 的面板约 5 分钟后自动出现新卡，不用发面板版。

## 条目格式

```json
{
  "id": "my-theme",
  "title": "My Theme",
  "cover": "https://raw.githubusercontent.com/<owner>/<repo>/<branch>/docs/preview.png",
  "tags": ["Minimal"],
  "description": {
    "zh-CN": "主题简介（中文）",
    "en": "Theme description (English)"
  },
  "url": "https://github.com/<owner>/<repo>",
  "branch": "build",
  "author": "<作者名>"
}
```

- `url` + `branch` 必须指向**构建产物**（`index.html` + `assets/`），不要指源码分支。
- 封面用 GitHub raw 图。
- 主题开发规范见 [ProbeDeck/theme-develop.md](https://github.com/gg949/ProbeDeck/blob/main/theme-develop.md)。

提交方式：提 PR 或开 issue。维护者会把新条目接到现有列表后面。
