# Smart-Location-DSS

> **元智大學 資訊管理學系 大四課程專案**
> **擔任組長並主導完整決策模型設計與系統開發**

這是一個結合 **Google Maps API** 與 **多準則決策分析 (MCDM)** 的互動式決策工具。本系統整合了 **AHP 層級分析法** 與 **TOPSIS 排序法**，旨在為創業商家提供科學化的實體店面設點評估。

### 📺 系統演示 (System Demo)

點擊圖片觀看系統操作演示 (權重設定 -> 地點模擬 -> 決策排序)：

[![DSS Demo Video](https://img.youtube.com/vi/YPZCVL7keUE/0.jpg)](https://www.youtube.com/watch?v=YPZCVL7keUE)

---

### 💡 核心優點與科學嚴謹性 (Key Features & Rigor)
* **科學化的權重推導 (AHP Rigor):**
     透過向 5 位受測者(組員)蒐集問卷，計算出五大指標權重：**商圈成熟度 (0.413)**、**交通便利度 (0.262)**、**人口密度 (0.139)**、**租金成本 (0.097)**、**競爭者密度 (0.089)** 。
* 經過計算，模型之**一致性比率 (Consistency Ratio, CR) = 0.041**，遠低於臨界值 0.1，證實決策權重具備高邏輯一致性 。
* **多維度決策排序 (TOPSIS Algorithm):**
     利用前端 JavaScript 即時運算各候選地點與理想解的相對接近度 (Relative Closeness)，產出客觀排名。
* **靈敏度分析 (Sensitivity Analysis):**
     針對不同店面規模（如 8坪、10坪、12坪）進行模擬，驗證決策模型在不同情境下的穩定性（結果穩定呈現信義 > 大安 > 中山）。
* **動態視覺化介面:**
     整合 Google Maps API，以**熱力圖 (Heatmap)** 呈現選址潛力，讓抽象數據具象化。

### 🔧 技術堆疊 (Tech Stack)
* **Frontend:** `HTML5` `CSS3` `JavaScript (ES6)`
* **Visualization:** `Google Maps JavaScript API` (Map & Visualization Library)
* **Algorithms:** `AHP (Analytic Hierarchy Process)` `TOPSIS` (Pure JS Implementation)
* **Data Source:** 政府開放資料平台 (Open Data), Google Places

---

### 📚 專案文件 (Documentation)
本專案包含完整的演算法邏輯說明與系統分析報告：

* **📄 [專案開發報告 (Project Report)](決策系統Assignment.pdf)**：包含完整的 AHP/TOPSIS 數學模型推導。
* **📊 [系統分析簡報 (Slides)](決策系統分析.pdf)**：包含詳細的選址策略與靈敏度分析結果。
* **📁 [AHP 權重推導與一致性檢定表 (AHP Weight Calculation)](DSS_final_template_3.xlsx)**：成對比較矩陣 (Pairwise Comparison Matrix)、五大指標權重計算過程，以及一致性比率的完整檢算紀錄 。
