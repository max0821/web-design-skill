# web-design Skill

[English](README.md) · **繁體中文**

**版本：** 1.2.1  
**作者：** max0821  
**授權：** MIT License  
**商業使用：** 允許

`web-design` 是一套以視覺設計為核心的 Agent Skill，用於高品質網站設計與精準重建。流程包含漸進式需求收斂、視覺概念生成與核准、結構化拆解、素材規劃、視覺一致性、Responsive composition，以及 Render-based QA。

## 版權與授權

Copyright © 2026 max0821.

本專案採用 MIT License 授權，可用於：

- 商業使用
- 私人使用
- 修改
- 再散布

使用、修改或再散布本專案時，必須保留原始版權聲明與 MIT License 授權聲明。

完整授權條款請參閱 [LICENSE](LICENSE)。

## 核心流程

```text
Understand
→ Progressive Clarification
→ Art Direction
→ Visual Exploration
→ User Reaction
→ Approved Visual Target
→ Decompose
→ Coherence Contract
→ Resolve Assets
→ Implement
→ Render
→ Compare
→ Fix
→ Repeat
```

## 核准稿後的四向拆解

視覺稿核准後，Skill 會先拆成：

- **Block Map** — 頁面區塊、章節邊界與閱讀流。
- **Layer Map** — 圖層、圖片、重疊關係與 z-order。
- **Text Map** — 真實文案、文字層級、斷行與 live text。
- **Geometry Map** — 比例、anchor、crop region 與 negative space。

另外使用跨四個 Map 的 **Token Map**，統一管理字型、色彩、間距、圓角、陰影、動態等設計 token。

## 視覺一致性

Skill 會明確管理：

- Typography System 與中英文字型搭配
- Visual Grammar / 元件語言一致性
- Asset Style Contract
- Composition Continuity
- Focal Hierarchy / Attention Budget
- Image / Text Relationship
- Motion & Interaction Language
- Responsive Continuity
- Brand Drift Detection
- Visual Coherence QA

## 素材處理

每一個重要視覺 layer 都應先分類成：

- Live HTML / UI
- CSS / SVG
- 現有或裁切素材
- 局部重新生成乾淨素材
- 省略／簡化

一旦視覺稿或素材被核准，就進入 LOCK 狀態。若單一素材有問題，只重新生成最小必要素材，不應重新抽整張頁面，避免 target drift。

## 檔案內容

- `SKILL.md` — Skill 主流程與規則。
- `README.md` — 英文說明。
- `README.zh-TW.md` — 繁體中文說明。
- `LICENSE` — MIT License。
- `agents/openai.yaml` — ChatGPT Skill UI metadata。
- `references/design-system.md` — Design System 指南。
- `references/visual-qa.md` — 視覺 QA 指南。
- `references/workflow-examples.md` — Workflow 範例。

## 安裝

將 `web-design` 資料夾或打包 ZIP 上傳至支援 Agent Skills / ChatGPT Skills 的介面。

資料夾名稱與 `SKILL.md` 宣告名稱保持一致：

```yaml
name: web-design
```

## 版本辨識

版本號會同步在三個位置：

1. `SKILL.md` → `metadata.version`
2. `SKILL.md` 頂部可視的 `Version:`
3. `agents/openai.yaml` → `interface.short_description`

這樣可以快速確認目前真正載入的是哪個 Skill 版本。
