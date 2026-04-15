# Smart-Location-DSS
結合 Google Maps API 與 多準則決策分析 (MCDM) 的系統。系統整合了 AHP 層級分析法與 TOPSIS 排序法，協助商家在預備進行的地點進行科學化的設點評估。

### System Demo

點擊圖片觀看系統操作演示 (權重設定 -> 地點模擬 -> 決策排序)：

[![DSS Demo Video](https://img.youtube.com/vi/YPZCVL7keUE/0.jpg)](https://www.youtube.com/watch?v=YPZCVL7keUE)

---

### 💡 核心功能 (Key Features)
* **多準則權重設定 (AHP Concept):** 使用者可動態調整五大指標（人口密度、租金成本、交通便利性、競爭密度、商圈成熟度）的權重偏好。
* **即時決策排序 (TOPSIS Algorithm):** 前端即時運算 TOPSIS 演算法，計算各候選地點的相對接近度 (Relative Closeness) 並進行排名。
* **地理資訊視覺化 (Visualization):** 整合 Google Maps API，以熱力圖 (Heatmap) 與標記 (Marker) 呈現選址潛力與詳細數據。
* **動態模擬 (What-If Analysis):** 支援即時新增/修改候選地點數據，系統會自動重新計算排名，輔助情境模擬。

### 🔧 技術堆疊 (Tech Stack)
* **Frontend:** `HTML5` `CSS3` `JavaScript (ES6)`
* **Visualization:** `Google Maps JavaScript API` (Map & Visualization Library)
* **Algorithms:** `AHP (Analytic Hierarchy Process)` `TOPSIS` (Implemented in JS)
* **Data Source:** 政府開放資料平台 (Open Data), Google Places

---

### 📚 專案文件 (Documentation)
本專案包含完整的演算法邏輯說明與系統分析報告：

* **📄 [專案開發報告 (Project Report)](決策系統Assignment #2.pdf)**
    * 內容包含：系統架構 (System Framework)、資料ETL流程、AHP 與 TOPSIS 數學模型詳細推導。
* **📊 [系統分析簡報 (Slides)](決策系統分析.pdf)**
    * 內容包含：選址策略分析、靈敏度分析 (Sensitivity Analysis) 結果與介面設計理念。
