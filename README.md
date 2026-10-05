# GitHub Pages + Firebase 多人 A/B 派對遊戲

這版不用 Node.js、Express、Socket.IO 或 Vercel。
GitHub Pages 負責靜態網頁，Firebase Realtime Database 負責多人即時同步。

## 上傳到 GitHub
1. 建立一個新的 repository。
2. 將本 ZIP 解壓後的所有檔案上傳到 repository 根目錄。
3. 到 Settings → Pages。
4. Source 選 Deploy from a branch。
5. Branch 選 main，Folder 選 /(root)，按 Save。
6. 發布後網址會像：https://你的帳號.github.io/你的專案名稱/

## Firebase Rules
到 Firebase Console → Realtime Database → Rules，測試時可貼上 database.rules.json 的內容。
注意：此規則是公開讀寫，只適合測試。正式公開前應改用 Authentication / App Check 限制。

## 遊戲流程
大螢幕開 GitHub Pages 網址 → 自動建立房號與 QR Code → 手機掃碼輸入名字 → 主持人選類別與題數 → 系統自動補成 3 人以上奇數 → 手機 A/B 投票 → 大螢幕撞擊、計分 → 最後前三名。

## 類別
生活 / 食物 / 愛情 / 親情 / 綜合

## 題數
5 / 10 / 15 題
