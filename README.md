# 成語大挑戰 v3.8 多人搶答進階版

這是可上傳 GitHub Pages 的版本。

## 本版更新

1. 多人遊戲加入房間後自動進入等待室
2. 掃 QR Code 或邀請連結會自動帶入房號
3. 新玩家加入時即時顯示玩家清單與排名
4. 房主可設定題數、倒數秒數、分類、難度
5. 多人遊戲結束後顯示完整成績表
6. 房主可移除玩家、重設分數、關閉房間

## 上傳檔案

請把以下檔案上傳到 GitHub repository 第一層：

- index.html
- idioms.js
- README.md
- manifest.json
- service-worker.js
- firestore.rules

請保留你原本已設定好的 firebase-config.js，不要覆蓋。

## Firebase Rules

本版若要使用「移除玩家」功能，請到 Firebase Console 的 Firestore Rules 貼上 `firestore.rules` 的內容並發布。
