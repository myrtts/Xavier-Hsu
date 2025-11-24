# 語言鍵使用與覆蓋報告

掃描範圍：workspace 內所有 `*.html` 檔案（搜尋 `data-lang="..."`）。

發現的 `data-lang` keys（依使用頻率/出現檔案）：

- nav-home
- nav-about
- nav-portfolio
- nav-contact
- hero-title
- hero-subtitle
- hero-desc
- btn-more
- info-title
- info-photo
- info-coding
- info-coffee
- skills-title
- contact-title
- contact-desc
- form-name
- form-email
- form-message
- btn-send
- footer-text
- p1-title
- p1-subtitle
- p1-desc-1
- p1-desc-2
- p2-title
- p2-subtitle
- p3-title
- p3-subtitle
- features
- f1
- f2
- f3
- f4
- f5
- tech-stack
- about-project
- btn-live
- btn-repo

比對來源：`js/langs.json`（包含 `en`、`zh`、`jp`、`kr`）。

結果：

- 在 `js/langs.json` 中，以上所有 keys 在四種語言（`en`、`zh`、`jp`、`kr`）均有對應翻譯。
- 因此目前沒有檢出「缺少翻譯鍵」的情況。

建議：

- 若日後新增頁面或改用新 key，請先在 `js/langs.json` 新增該 key 的翻譯，或使用下列自動掃描腳本來再次檢查。
- 若你偏好將某一語系 inline（以避免首屏閃爍），推薦把該語系少量常用字直接放在 HTML 或 `script.js`（目前我們已把完整四語放入 script 做 fallback）。

如需，我可以：

- 1) 產生 CSV/JSON 格式的覆蓋報告（可供給譯者使用）。
- 2) 自動把缺漏 key 加入 `js/langs.json`（以預設英文內容占位），供你後續翻譯。 

報告生成時間：2025-11-24
