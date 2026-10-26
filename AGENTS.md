# AGENTS.md

## 项目性质

纯静态 HTML/CSS 学生课程作业，无构建工具、无依赖、无包管理器。

## 关键约定

- 所有页面独立可用浏览器直接打开，无需本地服务器
- `index.html` 为入口页面，链接到所有练习文件
- 文件命名规则：`章节号-序号.html`（如 `11-1.html` 对应第 11 章第 1 个练习）
- 禁止使用 CDN 或外部依赖（页脚明确标注 "No CDN"）
- 只使用原生 HTML、CSS、JavaScript 实现，禁止引入第三方库或框架
- 图标必须使用 `fonts/` 目录下的 iconfont 图标（引用 `fonts/iconfont.css`，如 `<i class="iconfont">&#xe60a;</i>`），禁止使用 Font Awesome、Lucide 等第三方图标库
- 样式以 `<style>` 内联为主，仅 `5-1.html` 引用了 `css.css`
- 中文内容，`lang="zh-CN"`，字体优先使用 "Microsoft YaHei"
- 新建的 HTML 文件必须包含返回首页 `index.html` 的超链接
- 所有 CSS 类名、id 名、JS 变量必须以 `tang_` 开头
- 新建 HTML 文件时必须包含注释：`<!-- 作者：唐翊斌，建立时间：YYYY-MM-DD HH:MM，使用模型：XXX，功能名称：XXX -->`（建立时间为文件创建时间，使用模型为创建该文件时所用的大模型名称，功能名称为该页面的功能描述）
- 每次执行任务前，先将用户提示词追加写入 `tang_prompt.md`（不覆盖已有内容），格式包含：时间戳、使用的模型、提示词原文
- `tang_prompt.md` 分隔格式：每条记录以 `---` 分隔，标题行格式为 `## YYYY-MM-DD HH:MM | Model: <模型名>`
