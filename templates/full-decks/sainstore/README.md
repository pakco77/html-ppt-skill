# SainStore Weekly Report

基于 `weekly-report` 改造的 SainStore 品牌 deck，遵循 SainStore 视觉 DNA。

## 视觉规范

| 角色 | HEX | 用途 |
|---|---|---|
| 主红 | `#E7380D` | 强调、主标题、关键节点 |
| 主蓝 | `#1D7FB7` | 表头、节点、辅助强调 |
| 主黄 | `#F5AB18` | 流程节点、装饰圆环、编号 |
| 暖米底 | `#EFEAE0` | 页面背景（非纯白） |
| 主文字 | `#3D3935` | 偏暖深灰 |

字体：中文微软雅黑，英文/数字等线无衬线 / JetBrains Mono。

## 标志性元素

- **三色圆环（hollow rings）**：封面右侧大装饰圈、内页角落小装饰圈
- **撞色矩形条**：每页顶部 8px 红蓝黄三段，封面顶/底 14px 加粗
- **流程节点**：圆形+编号+连接虚线，边框红蓝黄循环用色（第 3 页）

## 页面结构（8 页）

1. **Cover** — 三色圆环装饰 + Logo + 大标题
2. **KPIs** — 8 宫格核心指标，左侧色条区分类型
3. **Pipeline** — 5 节点流程图（标志性三色圆环）
4. **Shipped** — 本周交付 6 项，FEAT/EXP/FIX/INFRA 标签
5. **Metrics** — GMV 8 周柱状图（最新一周高亮红色）
6. **Blockers** — 阻塞项卡片（左侧红条）
7. **Next Week** — 下周计划，右下角三色装饰环
8. **Thanks** — 渐变文字 + Logo 居中

## 用法

```bash
open templates/full-decks/sainstore/index.html
```

按 `←` `→` 翻页，`F` 全屏，`S` 演讲者模式（4 卡片磁吸视图）。

## 文件

- `index.html` — 8 页 deck 结构
- `style.css` — `.tpl-sainstore` 作用域，覆盖全局 token
- `logo.png` — SainStore 横版 Logo（1074×239 透明底）

## 替换内容

把 `index.html` 里的中文文案、KPI 数字、ship-item 列表换成你自己的就行，
所有视觉元素由 `.tpl-sainstore` CSS 自动套用。
