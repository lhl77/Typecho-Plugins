# Typecho 插件集合 - GitHub Pages

这个仓库包含一个用于展示 Typecho 插件集合的静态网站，风格参考 Material Design 3。网站托管在 GitHub Pages，内容位于 `docs/` 目录。

结构：

- `docs/index.html` - 站点主页
- `docs/style.css` - 主题样式（Material Design 3 风格）
- `docs/plugins.json` - 插件数据（JSON 数组）

快速开始：

1. 修改 `docs/plugins.json`，添加或更新你的插件信息。
2. 将代码推送到 GitHub。打开仓库设置 -> Pages，选择 `docs/` 目录作为源（或在 `main` 分支上启用 `docs/`）。
3. 等待几分钟，站点将在 `https://<your-user>.github.io/<repo>/` 上可访问。

如何自定义：

- 更改 `docs/style.css` 调整主题颜色或风格。
- 在 `index.html` 中引入更多字段（例如安装说明、版本、演示链接）并调整卡片模版。

搜索实现：
使用 Fuse.js 在客户端对 `plugins.json` 进行模糊搜索。可通过修改 `index.html` 中的 `options` 来调整搜索权重和阈值。

后续建议：

- 增加一个小的脚本来自动从 GitHub API 拉取插件仓库的 stars、最后更新信息。
- 增加分页、大量数据下的懒加载或服务器端搜索以提高性能。
