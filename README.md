# seo-geo-skills

Claude Code 用の SEO / GEO skill 6 本（中文）。

| skill | 用途 |
|---|---|
| `money-keywords` | 找有成交意图的关键词模式，输出 `keywords.md` |
| `page-brief` | 单关键词页面 brief，先判断新建还是优化 |
| `ship-page` | 按 brief 出页并发布，发布前过差异检查 |
| `geo-queries` | 生成 AI 助手会搜的查询，核对本站是否在榜 |
| `self-rank-audit` | 审计并改写"自己排第一"的榜单页 |
| `weekly-seo` | 周一复盘，输出 5 个行动项 |

## 安装

把需要的文件夹复制到 `.claude/skills/` 下（项目内或 `~/.claude/skills/`），新开会话即可使用。

下载整包：页面右上 **Code → Download ZIP**。

## 说明

- 工作流思路参考 Nicholas Dulait 的 X 长文「How to use Claude Opus 5.5 for SEO so well it feels illegal」（2026）。本仓库是按该思路自行改写的版本，不是原文。
- 原文依赖 ChatSEO MCP 取数据；未接入时各 skill 内写了替代数据源（Search Console 导出、Ahrefs、实时 SERP）。
- 未经实际运行验证。
