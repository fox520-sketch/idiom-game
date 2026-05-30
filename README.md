# 成語大挑戰 v4.0 多人遊戲正式版

這是可上傳到 GitHub Pages 的成語填空八選一學習遊戲，包含單人練習、快速遊戲、每日挑戰、考試模式、題庫學習、PWA 離線功能，以及 Firebase 多人搶答。

## v4.0 新增重點

1. 多人等待室加入「準備 / 取消準備」狀態。
2. 玩家清單會顯示房主、已準備、未準備。
3. 房主開始遊戲前會提醒尚未準備的玩家。
4. 多人遊戲中房主可手動「下一題」。
5. 多人遊戲中房主可手動「結束本局」。
6. 完整成績表可一鍵複製，方便貼到 LINE 或紀錄。
7. 保留 Firebase 匿名登入安全版規則。
8. 保留 QR Code 邀請、同房再玩一局、房主設定題數/秒數/分類/難度。

## 上傳 GitHub

請把以下檔案放在 repository 第一層：

- index.html
- idioms.js
- README.md
- manifest.json
- service-worker.js
- firestore.rules

請保留你原本已經填好的 `firebase-config.js`，不要覆蓋。

## Firebase

請確認已開啟：

- Authentication → Anonymous
- Firestore Database
- Firestore Rules 已更新為本版 `firestore.rules`

## 版本

程式版本：v4.0
題庫：約 891 題
