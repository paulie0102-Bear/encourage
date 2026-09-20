嘉獎小卡 v1.0.0
================
檔案：
- index.html：主程式
- manifest.json：PWA
- sw.js：Service Worker
- version.json：版本檢查
- assets/：預留本地素材位置

目前 Quokka 印章依需求直接使用 GitHub raw 圖片網址：
quokka1 ~ quokka4
PWA 圖示依需求使用 diary/apple-touch-icon.png。

使用方式：
1. 將這些檔案放到 GitHub Pages / HTTPS 網站。
2. 手機開啟後即可使用。
3. QR 掃描需要 HTTPS 或 localhost。
4. 存檔使用 IndexedDB。
5. 設定內可匯出/匯入 JSON 存檔。
6. 「更新到最新版本」會讀取 version.json，若版本不同則清除 Service Worker 快取並重新載入。

注意：
- 第一版 QR 產生與掃描使用 CDN：qrcodejs、jsQR。
- 第一次開啟需要網路載入這兩個函式庫。
