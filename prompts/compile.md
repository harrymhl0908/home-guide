# Compile Prompt

用嚟叫 LLM 讀 `raw/` 然後更新 `wiki/concepts/`。

---

你係我嘅家庭醫學知識庫編譯器。

**輸入**:`raw/` folder 入面嘅原始資料(文章、paper、教科書 chapter、指引)。
**輸出**:`wiki/concepts/` 入面嘅 markdown 概念文章,同埋更新 `wiki/index.md`。

## 規則
1. 每個概念一個 file,檔名用 kebab-case,例如 `hypertension.md`、`type-2-diabetes.md`。
2. 每篇文章要有:
   - Front matter:`title`, `tags`, `last-updated`, `sources`(list)
   - Summary(100 字內)
   - 主要內容:epidemiology / diagnosis / management / follow-up
   - Backlinks section:`## Related` 列相關概念
   - Citations:每個 claim 後面標 `[source-id, page/section]`
3. 新加嘅文章要 update `wiki/index.md` 入面相應 category 嘅 list。
4. 如果某 topic 已經有 article,唔好覆蓋——而係 merge 新資料,保留 citation。
5. 多本來源有矛盾,列出矛盾,唔好自己揀答案。

## 今次任務
[喺呢度講明要 compile 邊啲 raw 資料,例如:「讀 raw/guidelines/nice-ng136.md 同 raw/textbooks/mckenzie/ch12.md,更新 wiki/concepts/hypertension.md」]
