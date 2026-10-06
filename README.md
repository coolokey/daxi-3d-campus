# 桃園市立大溪國中 3D 智慧校園導覽與路徑導航系統 🏫
> **Ta-Yung / Daxi Junior High School 3D Smart Campus & Indoor Navigation**  
> 依據 115 學年度校園平面圖製作，採用輕量化 WebGL / Three.js 幾何參數化技術開發。

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-success?logo=github)](https://coolokey.github.io/daxi-3d-campus/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🌟 系統特色與核心技術

1. **極致輕量化參數建模（Procedural 3D Modeling）**：
   - 無需下載數十 MB 的笨重 3D 模型檔（如 GLTF / OBJ），直接使用純 JavaScript 依據平面圖幾何參數即時建構。
   - 全站原始碼與資源僅約數百 KB，在手機與電腦端均可次秒級秒開。
2. **兩種完整體驗模式**：
   - **模式一：全校 3D 鳥瞰漫遊與分層剖切（首頁模式）**
     - 自由 360 度俯瞰大溪國中校園、運動場、各棟大樓立體標籤。
     - 支援 1F / 2F / 3F / 4F 單樓層剖切檢視，清楚掌握室內隔間。
     - 支援第一人稱走廊漫遊（桌機 WASD 鍵盤 + 手機觸控虛擬搖桿）。
     - 左下角 2D 畫布即時動態小地圖（Minimap）。
   - **模式二：指定教室精準導航（`?to=教室代號` 深度連結模式）**
     - 適用於校園 QR Code 掃描、家長日尋路、新生報到、校慶導覽。
     - 透過 **A* 最短路徑演算法**，自動從校門口規劃跨樓層立體導航路線，並以 3D 發光黃色路徑指引。
3. **動態教室管理編輯器（Editor CMS）**：
   - 內建側邊抽屜式管理面板，支援每學年度班級教室名稱即時修改、本機快存（localStorage）與一鍵匯出 JSON。

---

## 🔗 常用深度導航連結範例（Deep Linking）

只要在網址後方加入 `?to=代號`，系統便會自動鎖定目標並開啟 3D 尋路導引：

| 目的地 | 網址參數連結 | 所在棟舍與樓層 |
| :--- | :--- | :--- |
| **教務處** | `?to=academic` | 行政大樓 2F |
| **校長室** | `?to=principal` | 行政大樓 2F |
| **健康中心** | `?to=health` | 行政大樓 1F |
| **701 教室** | `?to=701` | 七年級新大樓 1F |
| **706 質數研究室** | `?to=706` | 七年級新大樓 3F |
| **數學研究室** | `?to=math-lab` | 七年級新大樓 3F（蔡之民老師） |
| **801 教室** | `?to=801` | 八年級教學棟 2F |
| **901 教室** | `?to=901` | 九年級教學棟 3F |
| **科技創客館** | `?to=tech-lab` | 科技館 2F（張致信老師） |
| **樂活圖書館** | `?to=library` | 綜合大樓 2F |
| **學生活動中心** | `?to=gym` | 學生活動中心 1F |

---

## 🚀 部署說明

本專案為純前端靜態架構，可直接發布於任何靜態伺服器（GitHub Pages、Vercel、Cloudflare Pages 等）：

```bash
# 本地預覽
npx serve .
# 或使用 Python
python -m http.server 8080
```
