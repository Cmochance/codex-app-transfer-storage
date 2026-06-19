# codex-app-transfer-storage

Codex App Transfer 的插件/连接器市场**展示目录镜像**(private,仅供 transfer 拉取)。

镜像自 OpenAI Codex 的插件目录 `GET /backend-api/ps/plugins/list`(178 个连接器),按分类组织。

> **仅展示数据**(名称/分类/描述/图标/官网/示例 prompt)。这些连接器是 OpenAI 平台的 OAuth 远程连接器,由 OpenAI 单一 `plugin-runtime` MCP server(`chatgpt.com/backend-api/ps/mcp`)统一 broker、无独立 MCP 端点,故本镜像**仅用于市场浏览展示**,不含可连接的 MCP 配置。

## 结构
- `registry.json` — 连接器目录(178 个;图标指向本地 `icons/`,少量下载失败的保留原 OpenAI CDN URL 兜底)
- `icons/` — 镜像的图标 PNG(368 个)

## 每个连接器字段
`id` / `name` / `display_name` / `category` / `category_id` / `short_description` / `long_description` / `developer_name` / `brand_color` / `website_url` / `logo_url`(本地)/ `composer_icon_url`(本地)/ `default_prompts` / `status` / `version`

## 分类(10)
Productivity · Developer Tools · Finance · Business & Operations · Data & Analytics · Creativity · Communication · Education & Research · Other · Travel

镜像时间:2026-06-19 · 源:OpenAI Codex Desktop 0.142.0-alpha.1
