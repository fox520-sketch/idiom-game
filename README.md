# 成語大挑戰 v3.7.7 多人搶答題庫擴充版

本版為 GitHub Pages 上傳專用版。

## v3.7.7 更新重點

1. 多人搶答遊戲結束後，可在同一個房間繼續下一局。
2. 房主在結束畫面會看到「房主再玩一局」按鈕。
3. 再玩一局會重新抽題、重新計分、保留同一個房號與玩家。
4. 修正舊局答案可能影響新局搶答狀態的問題。
5. 保留答對即鎖題、自動下一題、只有答對者得分。
6. PWA 快取版本更新為 v3.7.7。

## 上傳 GitHub 檔案

請把下列檔案上傳到 repository 第一層：

```text
index.html
idioms.js
README.md
manifest.json
service-worker.js
firestore.rules
```

如果你的 `firebase-config.js` 已經填好 Firebase 設定，請不要覆蓋它。

## Firebase Rules

若多人搶答出現 Missing or insufficient permissions，請到 Firebase Console 的 Firestore Rules 確認允許 `idiomRooms`、`players`、`answers` 的讀寫。

## 快取提醒

上傳新版後如果仍看到舊版，請在網頁內按「立即更新」，或清除瀏覽器快取後重新開啟。
