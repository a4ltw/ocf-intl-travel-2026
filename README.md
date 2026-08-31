# 國際會議獎助計畫

OCF「國際會議獎助計畫」2026 年度徵選網站。純 HTML/CSS/無框架，用原生表單欄位（`name="entry.xxxx"`）直連 Google Form 的 `formResponse` 端點送出，Google Form 自動寫入其連結的 Google Sheet。

- `index.html` — 申請辦法（同時作為網站首頁，靜態內容對應內部 OPF4 D 子項目「2026徵選辦法草稿」）
- `apply.html` — 報名表單（原生欄位直連 Google Form）
- `recommend.html` — 國際會議推薦表單（原生欄位直連 Google Form）
- `gform-submit.js` — 共用的表單送出邏輯（fetch no-cors POST）

## 本地預覽

直接在瀏覽器開 `index.html` 即可。

## 部署

GitHub Pages，來源分支 `main` 根目錄。

## 資料來源

- 報名表單：OCF 國際盤纏計劃 2026 報名表單（Google Form，回覆寫入「OCF 國際盤纏計劃 2026 報名表單 (回覆)」試算表）
- 推薦表單：OCF 國際會議推薦表單（Google Form，回覆寫入「OCF 國際會議推薦表單 (回覆)」試算表）

兩份 Google Form 與回覆試算表皆存放於 OCF 內部 Google Drive「2.專案執行／[D]國際盤纏計劃 - Amos」資料夾，非本 repo 管理範圍。若表單題目改動，`apply.html`／`recommend.html` 裡的 `entry.xxxx` 欄位 ID 需要重新抓取對應更新。
