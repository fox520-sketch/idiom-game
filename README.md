# 成語大挑戰 v3.7.3 多人搶答鎖題版

這是可部署到 GitHub Pages 的成語填空八選一學習遊戲。

## v3.7.3 更新重點

1. 新增多人連線搶答。
2. 使用 Firebase Firestore 開房間。
3. 可建立房間、加入房間、複製邀請連結。
4. 同步題目與倒數時間。
5. 每位玩家個別計分。
6. 即時顯示排行榜與本題作答狀態。
7. 有人答對後立即鎖定本題，其他玩家不能再答。
8. 房主自動跳到下一題，只有答對者取得該題分數。

## 保留功能

- 800 題成語題庫
- 八選一作答
- 一般遊戲 / 快速遊戲 / 每日挑戰 / 考試模式
- 錯題本、智慧複習、弱點分析
- 收藏成語、我的成語筆記
- 匯出 / 匯入學習紀錄
- 練習卷 / 答案卷與列印
- 老師出題模式、自訂題庫匯入、題庫管理工具
- 離線可用 PWA
- 本機排行榜
- 題庫品質檢查

## 上傳 GitHub Pages

請把以下檔案放在 repository 第一層：

```text
index.html
idioms.js
README.md
manifest.json
service-worker.js
firebase-config.js
```

`.gitignore` 可以不用上傳。

## 多人連線 Firebase 設定

多人搶答需要 Firebase Firestore。

1. 到 Firebase Console 建立專案。
2. 建立 Web App。
3. 複製 Firebase SDK 設定中的 `firebaseConfig`。
4. 打開 `firebase-config.js`，把裡面的「請填入」改成你的 Firebase 設定。
5. 在 Firebase Console 啟用 Firestore Database。
6. 測試階段可以參考 `firestore.rules.example` 的規則。正式公開前建議再收緊規則。

## 注意

Firebase config 不是資料庫密碼，可以放在前端；真正要保護資料庫，需要靠 Firestore Rules。

本版多人搶答是輕量版，適合同一群朋友或教室內使用。如果要做公開大型對戰，建議之後再加入登入、房主權限驗證與更嚴格的資料庫規則。

## PWA 更新提醒

本版有 PWA 離線快取。如果上傳新版後看到舊畫面，請按網頁中的「立即更新」，或到「版本 / 除錯資訊」按「清除快取並重新載入」。


## v3.7.3 權限修正提醒
如果多人搶答出現「Missing or insufficient permissions」，請到 Firebase Console → Firestore Database → Rules，貼上 `firestore.rules` 的內容並 Publish。
注意：重新上傳本壓縮檔時，請保留你已填好的 `firebase-config.js`，不要把它覆蓋成範例設定。


## v3.7.3 更新

- 優化多人搶答規則。
- 有人答對後，Firestore 會鎖定該題。
- 其他玩家不能再送出同一題答案。
- 房主端會自動切換到下一題。
- 只有答對者取得該題分數。
