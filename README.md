# 🧠 PhysioMaster v6.3

> **專為物理治療師、運動教練與解剖學學生打造的智能化互動學習工具。**

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-success?style=flat-square&logo=github)](https://tonywen0012.github.io/physio-learning/)
[![Tech Stack](https://img.shields.io/badge/Built%20With-React%20%7C%20Tailwind-blue?style=flat-square&logo=react)](https://reactjs.org/)
[![AI Powered](https://img.shields.io/badge/AI-Google%20Gemini-orange?style=flat-square&logo=google)](https://ai.google.dev/)

## 📖 專案簡介 (Introduction)

**PhysioMaster** 是一個基於網頁的解剖生理學學習助手。它採用了 **Single File Component (SFC)** 架構，將 React 邏輯、Tailwind 樣式與龐大的解剖資料庫整合在單一 HTML 檔案中，實現了極致的輕量化與便攜性。

本工具結合了 **間隔重複系統 (SRS)** 與 **生成式 AI (GenAI)** 技術，旨在幫助使用者高效記憶肌肉起止點、神經支配及臨床測試動作。

🚀 **[點擊這裡立即開始使用 (Live Demo)](https://tonywen0012.github.io/physio-learning/)**

---

## ✨ 核心功能 (Features)

### 1. 🤖 AI 驅動的學習體驗
- **AI 臨床情境題**：串接 Google Gemini API，即時生成無限變化的臨床案例，測試你的鑑別診斷能力。
- **AI 智能助教**：答錯題目時，AI 會提供好記的口訣或臨床判斷點，幫助你理解而非死記。
- **智能填寫**：新增肌肉資料時，輸入名稱即可由 AI 自動填寫起止點與動作資訊。

### 2. 🧠 SRS 間隔重複記憶系統
- 內建 **SM-2 演算法**（類似 Anki），根據你的答題熟練度自動安排複習時間。
- 設有「今日複習」與「錯題本」模式，針對弱點精準打擊。

### 3. 📚 完整的解剖資料庫
- 收錄上百條肌肉與骨骼數據（包含起點、止點、神經、動作、臨床意義）。
- 支援關鍵字搜尋與分類篩選（上肢、下肢、軀幹、頭頸）。
- 支援 **Markdown 導入/導出**，方便備份學習進度或跨裝置轉移資料。

### 4. 🎓 主題課程模式
- 結構化的學習路徑（如：旋轉肌袖專題、步態肌群分析）。
- 循序漸進的解鎖機制與星級評分系統。

### 5. ⚡ 極致輕量與隱私
- **零後端**：所有資料與進度皆儲存於瀏覽器的 `localStorage`。
- **離線可用**：除 AI 功能外，基礎題庫與查詢功能皆可離線使用。

---

## 🛠️ 技術架構 (Tech Stack)

本專案是一個單頁應用程式 (SPA)，完全運行在客戶端瀏覽器中。

* **Core Framework**: React 18 (via CDN)
* **Styling**: Tailwind CSS (via CDN)
* **Transpiler**: Babel (via CDN)
* **Icons**: Lucide React
* **AI Integration**: Google Gemini API (`gemini-1.5-flash` / `gemini-1.5-pro`)
* **Storage**: Browser LocalStorage

---

## 🚀 如何使用 (How to Use)

### 線上使用
直接訪問 [GitHub Pages 連結](https://tonywen0012.github.io/physio-learning/) 即可開始。

### 啟用 AI 功能
若要使用 AI 臨床題與助教功能，你需要一組 Google Gemini API Key：
1.  前往 [Google AI Studio](https://aistudio.google.com/app/apikey) 免費申請 API Key。
2.  在 PhysioMaster 首頁輸入 Key 即刻啟用。
3.  *注意：API Key 僅儲存於您本地瀏覽器，不會上傳至任何伺服器。*

### 本地開發/部署
由於這是單一 HTML 檔案，部署極其簡單：
1.  Clone 此倉庫：
    ```bash
    git clone [https://github.com/TonyWen0012/physio-learning.git](https://github.com/TonyWen0012/physio-learning.git)
    ```
2.  直接用瀏覽器打開 `index.html` 即可運行。

---

## 📂 資料備份與同步 (Data Sync)

由於本工具使用 **LocalStorage**，資料是跟隨裝置與瀏覽器的。
* **更換裝置時**：請在舊裝置點擊「資料庫」->「導出」，將 `.md` 檔案傳送至新裝置，再點擊「導入」即可回復進度。
* **建議**：定期導出備份，以免瀏覽器快取被清除導致學習記錄遺失。

---

## ⚠️ 免責聲明 (Disclaimer)

本工具僅供解剖學學習與複習輔助使用。臨床醫療決策請務必遵循專業醫療指引與診斷流程。

---

**Created by Tony**
