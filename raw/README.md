# raw/ — Source Material Staging

呢個 folder 淨係放原始資料。LLM 會**讀**呢度,但唔會**寫**入呢度。

## Subfolders
- `articles/` — Obsidian Web Clipper 剪下嘅網上文章(.md + 下載嘅圖)
- `papers/` — PubMed / arXiv PDF(可 rename 做 `AuthorYear-keyword.pdf`)
- `textbooks/` — 每本書一個 folder,每 chapter 一個 `.md`
  - 例:`textbooks/mckenzie/ch12-hypertension.md`
- `guidelines/` — 臨床指引(NICE, AAFP, USPSTF, ESC, ADA 等)
- `notes/` — 自己手寫嘅臨床筆記 / case log

## 入料貼士
- 檔名用 kebab-case,帶年份同 topic,易 search
- 每個 file 開頭加返 front matter:`source`, `url`, `date-retrieved`,方便 LLM cite
- PDF 用 `marker-pdf` 或 `pymupdf4llm` 轉 markdown 先再擺入
