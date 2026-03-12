# aeo-demo-auto

## Overview
這是一個專為汽車產業設計的 AEO (AI-Evidence Optimization) 示範範本。專案展示了如何在傳統 HTML 網站中整合 Schema.org 結構化資料、llms.txt 檔案以及 FAQ 區塊，以提升內容被 AI 搜尋引擎索引的效率與正確性。

## Tech Stack
- **HTML5**: 頁面結構與語意標記。
- **JSON-LD**: 汽車相關產品的 Schema.org 結構化資料。
- **CSS3**: 基本樣式。
- **Plain Text**: 用於生成 `llms.txt` 供 AI 爬蟲讀取。

## Architecture
- **根目錄**: 包含主要 HTML 檔案 (`index.html`) 與 AI 索引檔案 (`llms.txt`)。
- **Assets**: 圖片與樣式表資料夾 (css/, images/)。
- **Data**: (可選) 用於存放產品結構化資料的 JSON 檔案。

## Commands
此為靜態網站，無需建置流程。
- **本地預覽**: 使用簡單的 HTTP 伺服器執行 `python3 -m http.server` 或透過 VS Code 的 Live Server 外掛。
- **驗證**: 使用 Google Rich Results Test 工具檢測 Schema.org 標記是否正確。

## Coding Style
- **語意化標籤**: 必須使用 `<article>`, `<section>`, `<header>` 等語意化標籤。
- **Schema 優先**: 在 `<head>` 中正確嵌入 JSON-LD 腳本。
- **AI 友善**: 確保文字內容清晰，避免過度依賴 JavaScript 加載關鍵資訊。

## Important Rules
- **嚴禁移除標記**: 不得刪除 `llms.txt` 或任何 Schema.org 結構化資料。
- **保持更新**: 當產品資訊變更時，必須同步更新 JSON-LD 資料。
- **robots.txt**: 確保允許 AI 機器人存取 `llms.txt` 與主要內容頁面。