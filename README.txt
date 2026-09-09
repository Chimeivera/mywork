個人工作管理系統 v6.0

【GitHub Pages 上傳】
只需上傳：
1. index.html
2. sw.js
3. manifest.webmanifest
4. icon-192.png
5. icon-512.png

Code.gs 不需要上傳 GitHub；它是提供給 Apps Script 使用。

【Apps Script】
1. 開啟綁定 Google Sheet 的 Apps Script。
2. 將 Code.gs 全部替換成此資料夾內 Code.gs。
3. 儲存。
4. 部署 → 管理部署作業 → 編輯 → 新版本 → 部署。
5. 保留原本 /exec 網址即可。
6. 打開 /exec?action=ping，確認 version 是 6.0.0。

【Google Sheets】
可直接使用隨附的 Google_Sheets_v6_資料庫範本.xlsx，上傳 Google Drive 後以 Google 試算表開啟。
也可以使用空白 Google Sheet；第一次呼叫 API 時 Code.gs 會自動建立：工作、案件、歷程、操作紀錄、設定。

【安全建議】
更新前先複製一份現有 Google Sheet 備份。v6 採軟刪除：工作/歷程刪除後仍保留 deletedAt，前端不再顯示。
