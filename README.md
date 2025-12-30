# BMad Skills

為 Claude.ai 網頁介面設計的 BMad 風格 Skills。

## 什麼是 Skills？

Skills 是教導 Claude 如何執行特定任務的 markdown 檔案。當你將 Skill 提供給 Claude 時，它會遵循指示以一致的行為完成專門任務。

> 這些 Skills 專為 **Claude.ai 網頁介面**設計。透過將結構化指示加入對話或專案中，讓 Claude 能夠扮演專業角色並執行特定工作流程。

更多關於 Skills 的資訊，請參閱：

- **[Skills 完整指南（繁體中文）](docs/skills-guide-zh-tw.md)** — 本專案整理的中文版指南
- [Agent Skills 概覽](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview)
- [快速入門指南](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/quickstart)
- [最佳實踐](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/best-practices)
- [在 Claude 中使用 Skills](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [教 Claude 按照你的方式工作](https://support.claude.com/en/articles/12580051-teach-claude-your-way-of-working-using-skills)

## 可用的 Skills

| Skill | 說明 |
|-------|------|
| [bmad-party-mode](skills/bmad-party-mode/) | 10 位 AI 專家的多 Agent 協作模式 |

## BMad Party Mode

多 Agent 協作系統，讓 10 位 AI 專家共同參與對話，提供多元觀點。

### 適用情境

- 技術架構討論與決策
- 產品策略規劃
- 專案腦力激盪
- 需要多角度專家意見的複雜問題

### 專家團隊

| 圖示 | 名稱 | 角色 | 專長領域 |
|------|------|------|----------|
| 🧙 | BMad Master | 協調者 | 流程引導、討論協調 |
| 📊 | Mary | 商業分析師 | 需求分析、市場研究 |
| 🏗️ | Winston | 架構師 | 系統設計、「無聊的技術」 |
| 💻 | Amelia | 開發者 | TDD、精準實作 |
| 📋 | John | 產品經理 | 策略規劃、優先排序 |
| 🚀 | Barry | 快速開發者 | 快速原型、全端開發 |
| 🏃 | Bob | Scrum Master | Agile 流程、Story 準備 |
| 🧪 | Murat | 測試架構師 | 測試策略、CI/CD、品質 |
| 📚 | Paige | 技術作家 | 文件撰寫、知識整理 |
| 🎨 | Sally | UX 設計師 | 使用者體驗、介面設計 |

### 觸發詞

- 「party mode」/「bmad party mode」
- 「開始 party mode」/「啟動 party mode」
- 「召喚團隊」/「召喚專家」
- 「團隊討論」/「專家會議」

### 運作方式

1. **主題分析**：識別討論領域（技術/商業/設計/流程）
2. **專家選擇**：挑選 2-3 位最相關的專家
3. **回應生成**：每位專家以獨特風格回應
4. **跨專家互動**：專家可以引用並延伸彼此觀點

## 安裝方式

### 方式一：上傳 ZIP 到 Claude Project（推薦）

1. 在 Claude.ai 建立新專案（Project）
2. 下載並壓縮 `skills/bmad-party-mode/` 資料夾為 ZIP 檔
3. 將 ZIP 上傳至 Project Knowledge
4. 開始對話並使用觸發詞

### 方式二：個別上傳檔案

1. 在 Claude.ai 建立新專案（Project）
2. 將以下檔案上傳至 Project Knowledge：
   - `skills/bmad-party-mode/SKILL.md`
   - `skills/bmad-party-mode/references/agents.md`
   - `skills/bmad-party-mode/references/rules.md`
3. 開始對話並使用觸發詞

### 方式三：直接對話

將 Skill 內容直接複製貼上到對話中作為 context。

## 檔案結構

```text
skills/
└── bmad-party-mode/
    ├── SKILL.md              # 主要 Skill 定義
    └── references/
        ├── agents.md         # 詳細 Agent 人格設定
        └── rules.md          # 選擇規則與指引
```

## 致謝

本專案靈感來自 BMad Code, LLC 的 [BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) — 一套以 AI 驅動的敏捷開發框架，具備專業化 AI Agent。

## 授權

MIT License

BMad™ 和 BMAD-METHOD™ 是 BMad Code, LLC 的商標。
