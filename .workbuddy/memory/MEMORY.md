# 项目长期约定与备忘（Duan516.github.io）

## 协作模式（必须遵守）
- **只读咨询模式**：不直接修改网站文件，只提供「文件路径 + 具体改动指令」，用户自行修改。

## 项目要点
- al-folio 学术模板，Jekyll + GitHub Pages
- 主页 = `_pages/sketches.md`（速写照片瀑布流，permalink: `/`），不是默认 about 页
- 简历数据在 `_data/cv.yml`（中文），简历页 `_pages/cv.md`，`cv_pdf` 指向作品集 PDF
- `_projects/` 4 个建筑作品（category: work）
- 模板示例残留：`_posts/`(30)、`_news/`(3)、`_books/`(1)、`about.md` 占位、`assets/bibliography/` 示例 bib、`resume.json` 半改
- scholar 配置未个性化（仍是 Einstein），论文功能未启用
- `_config.yml`: enable_darkmode: true，lang: en

## 主题改造要点
- 默认暗色：`assets/js/theme.js` `determineThemeSetting()` 中 `themeSetting = "system"` → `"dark"`
- 强调色：`_sass/_themes.scss` 中 `--global-theme-color` / `--global-hover-color`（暗色块当前为 cyan #2698ba）
- 暗色背景变量：`$grey-color-dark` = #1c1c1d（`_sass/_variables.scss`）

## 用户参考风格
- gxzv.com（甘小蔗）：暗色 + 文学性文案 + 大图 + 个人叙事 + 暖色点缀
