個人工作管理系統 v5.2
1. 先備份原本 Google Sheet（檔案 → 建立副本）。
2. Apps Script：以 Code.gs 取代原程式，儲存後部署新的網頁應用程式版本。保留原部署網址。
3. GitHub：上傳 index.html、sw.js、manifest.webmanifest、icon-192.png、icon-512.png，覆蓋同名檔案並 Commit。
4. 重新整理後確認右下角版本 5.2。先用測試工作驗證新增、編輯、刪除歷程及 Excel 匯出。
5. 刪除歷程採軟刪除，原始資料保留於 Google Sheet 的 deletedAt 欄位；網頁與報表不顯示已刪除紀錄。
6. 舊版已產生的重複紀錄不會自動刪除，請確認後逐筆清理。
7. 本版不需要 UrlFetchApp 匯出權限；Excel 由瀏覽器產生 .xls（Excel XML 格式）。
