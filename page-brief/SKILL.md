---
name: page-brief
description: 为一个目标关键词做 SEO 页面 brief。当被要求"把某个词做上去""优化某个页面"，或在新建任何页面之前使用。
---

# page-brief — 单关键词页面 brief

> 思路参考：Nicholas Dulait 的 X 长文（2026）里的同名 skill。本文件是按该思路自行改写的版本，不是原文。
> 数据源：原文依赖 ChatSEO MCP。未接入时改用 Search Console（查询 → 页面维度）+ 实时 SERP 抓取 + `keyword-researcher`。

## 原则

- 一个关键词只对应一个页面。先查有没有旧页，再决定新建还是优化，否则会自己和自己抢排名。
- 次要关键词 = 排第 1 的那个 URL 同时排进前 5 的其他查询。这些词用同一个 URL 一起打。
- 标题是页面最强的站内信号，一个词就能决定覆盖一个查询还是五个。meta description 主要负责拉点击。

## 步骤

1. 向数据源提问：目标是 `<keyword>` 排第一。请它读当前前 10，回答三件事：哪种页面类型在赢；前 3 名还同时排着哪些次要关键词；本站应优化已有页面还是新建。然后要完整 brief。
2. 等结果完整后提取：新建／优化及对应 URL、主关键词与次要关键词、前 3 名都有的版块、建议的 title 和 meta description。
3. 判定闸门：如果已有 URL 在这个词上有点击或曝光，**停止任何新建计划**，改为优化该页。
4. 检查标题：包含主关键词，并且在 SERP 预览里不会被截断。
5. 把 brief 存到 `briefs/<keyword-slug>.md`。这一步不改站点。

## 输出

`briefs/<keyword-slug>.md`（供 `ship-page` 读取）。
