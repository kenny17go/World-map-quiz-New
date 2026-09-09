# 世界地圖知識測驗 — GitHub Pages 版

這個資料夾可以直接部署到 GitHub Pages，不需編譯、不需 npm。

## 最簡單部署方式

1. 在 GitHub 建立一個新的 Repository，例如 `world-map-quiz`。
2. 把這個資料夾內的所有檔案上傳到 Repository **根目錄**。
3. 到 Repository 的 **Settings → Pages**。
4. 在 **Build and deployment**：
   - Source 選 **Deploy from a branch**
   - Branch 選 **main**
   - Folder 選 **/(root)**
   - 按 **Save**
5. GitHub Pages 建立完成後，用 Safari 開啟網址。
6. iPhone Safari 按 **分享 → 加入主畫面 → 加入**。

## iPhone 建議

- 建議橫向使用，世界地圖會有更大的操作區域。
- 第一次請保持網路連線並完整開啟一次；Service Worker 完成快取後，可支援離線再次開啟。
- 若更新網站後仍看到舊版，可關閉主畫面 App 後重新開啟；必要時從主畫面刪除後再重新加入。

## 檔案

- `index.html`：主程式、地圖與題庫，均已內嵌。
- `manifest.webmanifest`：PWA 設定。
- `service-worker.js`：離線快取。
- `icon-180.png`：iPhone 主畫面圖示。
- `icon-192.png` / `icon-512.png`：PWA 圖示。
- `.nojekyll`：讓 GitHub Pages 直接原樣提供靜態檔案。
