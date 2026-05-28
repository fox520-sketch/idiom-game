# 成語填空小遊戲 v2.2

這是一個可直接部署到 GitHub Pages 的成語填空網頁遊戲。

## 本版特色

- 預設固定四選一作答
- 答案按鈕加上 A / B / C / D 標示
- 選完後會標出正確答案與錯誤答案
- 增加每輪題數：10 題、20 題、30 題、全部題目
- 增加正確率
- 增加最佳分數，會保存在瀏覽器 localStorage
- 遊戲結束後顯示錯題複習
- 題庫獨立在 `idioms.js`
- 支援自然模式、深色模式、黑白模式
- 手機版按鈕較大，方便觸控
- 上方保留「回狐狸之家」連結

## 上傳 GitHub Pages

解壓縮後，請把以下檔案放到 GitHub repository 第一層：

```text
index.html
idioms.js
README.md
.gitignore
```

不要只上傳整個資料夾，否則 GitHub Pages 可能找不到首頁。
