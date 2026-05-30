# 成語大挑戰 v3.9 Firebase 匿名登入安全版

這是可上傳 GitHub Pages 的版本。

## 本版更新

1. 新增 Firebase Anonymous Authentication 匿名登入
2. 多人房間的 hostId 改用 Firebase 匿名使用者 UID
3. Firestore Rules 改為需登入後才能讀寫多人房間資料
4. 玩家只能更新自己的玩家資料與答案
5. 房主可管理房間、重設分數、移除玩家、關閉房間
6. 保留 v3.8 多人搶答進階版功能

## 上傳檔案

請把以下檔案上傳到 GitHub repository 第一層：

- index.html
- idioms.js
- README.md
- manifest.json
- service-worker.js
- firestore.rules

請保留你原本已設定好的 firebase-config.js，不要覆蓋。

## Firebase 必須新增設定

請到 Firebase Console：

Authentication → Sign-in method → Anonymous → Enable

然後到：

Firestore Database → Rules

貼上 `firestore.rules` 的內容並發布。
