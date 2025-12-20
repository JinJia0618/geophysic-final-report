# geophysic-final-report
# 🌍 113-1 地球物理通論 (General Geophysics) 期末專題成果

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-blue?style=for-the-badge&logo=github)

> **"Exploring the Earth through Physics"**
> 
> 本專案為 113 學年度第一學期「地球物理通論」課程之期末整合報告。利用現代化網頁技術 (React + Vite)，將抽象的地球物理原理轉化為**互動式視覺模擬**，並完整記錄野外實驗數據、Python PyGMT 實作與專家演講心得。

## 🔗 線上展示 (Live Demo)

👉 **[點擊進入互動式網站](https://jinjia0618.github.io/geophysic-final-report/)**

---

## 📚 專案核心模組 (Core Modules)

本平台整合了 10 大核心單元，涵蓋四大地球物理場與現代探勘技術：

### 1. 🔨 震測探勘實驗 (Seismic Refraction)
* **野外實作**：記錄校園折射震測實驗流程（24道檢波器佈設、人工震源激發）。
* **數據分析**：展示走時曲線 ($T-X$ Plot) 分析結果。
* **成果**：成功推算出校園地下雙層構造速度 ($V_1 \approx 427$ m/s, $V_2 \approx 593$ m/s) 與第一層厚度。

### 2. 📝 折射震測模擬 (Simulation & Derivation)
* **理論推導**：從司乃耳定律 (Snell's Law) 出發，完整推導臨界折射波走時方程式。
* **互動模擬器**：
    * 可調整參數：$V_1, V_2, h$ (震源深度)。
    * 即時計算：**臨界距離 ($X_{cr}$)** 與 **截距時間 ($T_i$)**。
    * 視覺化：動態繪製波傳遞路徑（直達波 vs. 頭波）。

### 3. ⚖️ 重力測勘原理 (Gravity Method)
* **校正模擬**：提供互動式滑桿，視覺化以下校正原理：
    * **自由空間校正 (FAC)**：$FAC = 0.3086 \times h$ (高度影響)。
    * **布格校正 (BC)**：$BC = 0.0419 \times \rho \times h$ (質量影響)。
* **異常解釋**：透過高斯曲線模擬，展示地下密度差異 ($\Delta\rho$) 如何形成重力正異常（礦體）或負異常（空洞）。

### 4. 🧲 古地磁學 (Paleomagnetism)
* **古緯度計算機**：實作 $\tan(I) = 2\tan(\lambda)$ 公式，輸入磁傾角即可反推板塊古緯度。
* **視極移曲線 (APWP)**：視覺化板塊還原過程，展示北美與歐亞板塊磁極路徑的重合現象，驗證大陸漂移學說。

### 5. 🔥 地球熱流 (Geothermics)
* **熱流計算**：基於傅立葉熱傳導定律 ($q = -k \frac{dT}{dz}$)，計算地表熱流值。
* **全球熱流地圖**：互動式地殼剖面，解析 **中洋脊 (High Heat Flow)**、**隱沒帶 (Low Heat Flow)** 與 **克拉通 (Stable)** 的熱特徵。

### 6. 🗺️ 板塊構造解析 (Plate Tectonics)
* **南極板塊專題**：聚焦於被擴張脊與海溝環繞的南極板塊構造。
* **PyGMT 實作**：
    * 整合 ETOPO1 地形資料與 USGS 地震目錄。
    * 展示 **Google Colab** 環境下的 PyGMT 繪圖優化成果（高解析地形渲染）。

### 7. ⚡ 地熱探勘與 AI 應用 (Geothermal & AI)
* **探勘方法**：介紹陸地鑽井與海洋探針 (Heat Flow Probe) 測量原理。
* **RAG 知識庫**：展示利用 **Dify** 平台建置的 AI 地熱問答機器人，結合專業文獻進行精準回答。

### 8. 💻 資訊實作與協作 (Coding & Collaboration)
* **GitHub Codespaces**：記錄利用雲端環境執行 ObsPy (地震波處理) 與 PyGMT (地圖繪製) 的流程。
* **Version Control**：透過 Pull Request (PR) 機制提交作業，體驗開源協作流程。

### 9. 🌐 網站整合成果 (Web Integration)
* **Google Blogger**：個人學術部落格與週記整合。
* **Hugging Face**：嵌入課程授課大綱與其他 AI 實作專案。

### 10. 🎤 專家演講心得 (Guest Lectures)
收錄本學期三場重要演講之重點筆記：
* **甘禮有 博士** (中研院)：地震層析成像與地球內部構造。
* **黃有志 教授** (台大)：地震災害與火山防災（熊本地震、阿蘇火山）。
* **廖勿渝 博士** (中油)：震測資料處理在能源探勘的應用。

---

## 🛠️ 技術架構 (Tech Stack)

本專案採用現代化前端技術構建，確保跨裝置的流暢體驗：

| Category | Technology | Usage |
|----------|------------|-------|
| **Core** | ![React](https://img.shields.io/badge/-React-20232A?logo=react) | UI 組件化開發 |
| **Build** | ![Vite](https://img.shields.io/badge/-Vite-646CFF?logo=vite) | 快速建置與打包 |
| **Styling** | ![Tailwind CSS](https://img.shields.io/badge/-Tailwind-38B2AC?logo=tailwind-css) | 響應式排版與深色模式 |
| **Icons** | ![Lucide](https://img.shields.io/badge/-Lucide-F05032) | 視覺化圖標庫 |
| **Deploy** | ![GitHub Pages](https://img.shields.io/badge/-GitHub%20Pages-222222?logo=github) | 靜態網站託管 |

---

## 🚀 本地執行指南 (Run Locally)

若需在本地端執行本專案，請依照以下步驟：

1.  **複製專案 (Clone)**
    ```bash
    git clone [https://github.com/JinJia0618/geophysic-final-report.git](https://github.com/JinJia0618/geophysic-final-report.git)
    ```

2.  **安裝相依套件 (Install)**
    ```bash
    cd geophysic-final-report
    npm install
    ```

3.  **啟動開發伺服器 (Dev)**
    ```bash
    npm run dev
    ```

---

## 👤 作者資訊 (Author)

* **姓名**：黃靖家 (JinJia Huang)
* **學號**：U11310017
* **系級**：台北市立大學 地球環境暨生物資源學系 (地科組) 二年級
* **課程**：113-1 地球物理通論
* **指導教授**：[老師名字]

---

*Last Updated: 2025/12/20*
