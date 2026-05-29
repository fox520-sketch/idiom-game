# 成語填空小遊戲 v2.8 題庫與注音擴充版

這是一個可直接部署到 GitHub Pages 的成語填空網頁遊戲。

## v2.8 更新

- 補齊既有題庫中空白的注音欄位。
- 題庫由 238 題擴充到 310 題。
- 保留快速遊戲設定：可選難度、分類、每輪題數、倒數時間與顯示風格。
- 保留固定四選一作答。
- 保留錯題本、學習紀錄、成語學習卡、注音欄位與分享成績。

## 上傳 GitHub Pages

解壓縮後，請把下列檔案放到 repository 第一層：

```text
index.html
idioms.js
README.md
```

`.gitignore` 可上傳也可不傳，不影響網站運作。

## 題庫修改方式

題庫集中在 `idioms.js`。新增題目時，請使用這種格式：

```javascript
{ full: "精益求精", blank: "精益求＿", answer: "精", hint: "更好", meaning: "已經很好還要追求更好。", level: "中等", category: "學習成語", zhuyin: "ㄐㄧㄥ ㄧˋ ㄑㄧㄡˊ ㄐㄧㄥ", example: "做事要精益求精。" }
```
