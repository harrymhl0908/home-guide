# Lint Prompt

每週跑一次,搵 wiki 入面嘅問題。

---

你係我嘅家庭醫學知識庫 linter。掃晒 `wiki/concepts/`,然後出 report 做 `wiki/lint-YYYY-MM-DD.md`。

## 檢查項目
1. **矛盾**:唔同文章之間有冇互相矛盾嘅 claim?
2. **過時**:有冇 citation 喺 5 年前以上,而相關領域有新 guideline?
3. **缺口**:index.md 列嘅 concept 有冇 article 未寫?常見 family medicine topic 有冇漏?
4. **孤兒**:有冇 article 完全冇 backlink?
5. **未 cite**:有冇 claim 冇標 source?
6. **可合併**:有冇兩篇 article 講緊同一樣嘢?
7. **新文章建議**:根據而家 wiki 嘅連結 pattern,建議 3-5 個新 article topic。

## 輸出 format
每一項用 bullet list,每個 issue 附:
- 檔案路徑 + 行號(如適用)
- 問題簡述
- 建議行動

最後 update `wiki/index.md` 嘅 "Lint Log" section,加一條記錄。
