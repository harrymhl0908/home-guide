# Home Guide — Family Medicine Knowledge Base

個人家庭醫學知識庫,用 LLM 做 compiler,將 `raw/` 入面嘅原始資料編譯成 `wiki/` 入面嘅結構化 markdown wiki。

## Quick Start
1. 將網上文章用 **Obsidian Web Clipper** 剪入 `raw/articles/`
2. PDF paper 擺入 `raw/papers/`
3. 教科書 chapter(一個 chapter 一個 `.md`)擺入 `raw/textbooks/<book-name>/`
4. 用 Obsidian 打開成個 repo 做 vault
5. 用 `prompts/` 入面嘅 prompt 叫 LLM 編譯 / 查詢 / lint

## Folder Layout
```
raw/          原始資料(LLM 只讀)
  articles/   網上剪下嘅文章
  papers/     學術論文
  textbooks/  教科書(每本一個 folder,每 chapter 一個 file)
  guidelines/ 臨床指引
  notes/      自己嘅臨床筆記

wiki/         編譯後嘅知識庫(LLM 會寫)
  index.md    總索引,入口
  concepts/   概念文章
  summaries/  來源摘要
  qa/         查詢答案

outputs/      衍生產物
  slides/     Marp slide decks
  charts/     圖表

prompts/      常用 prompt template
```

## Workflow
睇 [`wiki/index.md`](wiki/index.md) 做入口。

Pipeline 參考 Karpathy 嘅 LLM Knowledge Base 架構:**Ingest → Compile → Query → Lint → (loop)**.
