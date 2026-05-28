# 成語填空小遊戲

這是一個可直接部署到 GitHub Pages 的成語填空網頁遊戲。

## 功能

- 成語填空
- 輸入答案模式
- 四選一模式
- 難度篩選
- 分類篩選
- 隨機出題
- 不重複出題
- 提示功能
- 答案解釋
- 分數統計
- 自然模式、深色模式、黑白模式
- 手機版適配

## 檔案說明

```text
index.html   主程式與畫面
idioms.js    題庫資料
README.md    說明文件
.gitignore   Git 忽略設定
```

## 如何增加題目

打開 `idioms.js`，依照下面格式新增：

```javascript
{ full: "畫蛇添足", blank: "畫＿添足", answer: "蛇", hint: "一種爬行動物", meaning: "比喻多此一舉，反而壞事。", level: "簡單", category: "動物成語" }
```

## GitHub Pages

Repository 建議名稱：

```text
idiom-game
```

部署後網址通常會是：

```text
https://fox520-sketch.github.io/idiom-game/
```
