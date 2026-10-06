# 桃園市立大溪國中 3D 智慧校園導覽與路徑導航系統 🏫
> **Ta-Yung / Daxi Junior High School 3D Smart Campus & Indoor Navigation**  
> 依據真實空拍機實錄影像（DJI Mavic 2）與 115 學年度校園平面圖比對製作，採用輕量化 WebGL / Three.js 幾何參數化技術開發。

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-success?logo=github)](https://coolokey.github.io/daxi-3d-campus/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🚁 實境空拍影像忠實比對還原

本專案對比真實空拍機俯瞰影像，深度還原以下標誌性校園地標：
1. **學生活動中心 / 體育館**：
   - 還原溫潤的**粉紅鮭魚磚色（Salmon Pink）**外牆。
   - 入口右側特別建置標誌性的**圓柱狀雙塔樓梯井（Cylindrical Twin Towers）**與環狀採光窗。
   - 頂樓防水層中央設有大型圓形排氣機房通風設備。
2. **200 公尺綜合運動場（操場跑道）**：
   - 忠實還原實境**深碳灰/深青紫黑色 PU 跑道**（非傳統亮紅）。
   - 中央天然大草坪右側精確置入**雙排亮紅色排球/羽網球場**。
   - 司令台建置真實空拍所見之**鮮明亮紅色雙坡金屬斜屋頂（Red Gable Roof）**。
3. **教學大樓紅瓦斜頂**：
   - 右側教學大樓頂樓還原大溪國中辨識度極高的**金屬亮紅烤漆斜坡防漏屋面**。
4. **前庭迎賓大道與停車廣場**：
   - 鋪設灰白壓花地磚、黃色人行/減速斜紋警示帶、白色停車格線與校門金頂圓球門柱。
5. **校園西側綠水圳**：
   - 模擬活動中心外側防汛水圳渠道與斜坡混凝土駁坎。

---

## 🌟 核心功能特色

1. **極致輕量化**：全站純原生程式碼打包僅數百 KB，在手機與電腦端均可次秒級秒開。
2. **兩種完整體驗模式**：
   - **全校 3D 鳥瞰漫遊**：360° 旋轉縮放、1F~4F 樓層剖切透視室內隔間、第一人稱漫遊（WASD / 手機虛擬搖桿）、左下角 2D 即時動態小地圖。
   - **指定教室/場館深度導航（`?to=代號`）**：支援 A* 跨樓層室內最短路徑搜尋，自動在 3D 空間拉出立體發光導航黃色路徑。
3. **每學年班級編輯器（Editor CMS）**：內建抽屜管理面板，支援線上修改教室名稱、localStorage 快存與 JSON 備份。

---

## 🔗 實境地標深度導航測試連結

點擊下列連結即可在開啟網頁時直接啟動 3D 發光路徑導航：

| 地標 / 處室 / 班級 | 所在位置與樓層 | 深度導航測試網址 |
| :--- | :--- | :--- |
| **學生活動中心** | 西南側挑高體育館 1F | [👉 導航到活動中心 (`?to=gym`)](https://coolokey.github.io/daxi-3d-campus/?to=gym) |
| **操場司令台** | 200m 運動場南側紅斜頂小亭 | [👉 導航到司令台 (`?to=grandstand`)](https://coolokey.github.io/daxi-3d-campus/?to=grandstand) |
| **教務處** | 行政大樓 2F | [👉 導航到教務處 (`?to=academic`)](https://coolokey.github.io/daxi-3d-campus/?to=academic) |
| **校長室** | 行政大樓 2F | [👉 導航到校長室 (`?to=principal`)](https://coolokey.github.io/daxi-3d-campus/?to=principal) |
| **健康中心** | 行政大樓 1F | [👉 導航到健康中心 (`?to=health`)](https://coolokey.github.io/daxi-3d-campus/?to=health) |
| **701 教室** | 七年級新大樓 1F | [👉 導航到 701 教室 (`?to=701`)](https://coolokey.github.io/daxi-3d-campus/?to=701) |
| **706 質數研究室** | 七年級新大樓 3F | [👉 導航到 706 教室 (`?to=706`)](https://coolokey.github.io/daxi-3d-campus/?to=706) |
| **數學研究室** | 七年級新大樓 3F（蔡之民老師） | [👉 導航到數學研究室 (`?to=math-lab`)](https://coolokey.github.io/daxi-3d-campus/?to=math-lab) |
| **801 教室** | 八年級教學棟 2F | [👉 導航到 801 教室 (`?to=801`)](https://coolokey.github.io/daxi-3d-campus/?to=801) |
| **901 教室** | 九年級教學棟 3F | [👉 導航到 901 教室 (`?to=901`)](https://coolokey.github.io/daxi-3d-campus/?to=901) |
| **科技創客館** | 科技館 2F（張致信老師） | [👉 導航到科技創客館 (`?to=tech-lab`)](https://coolokey.github.io/daxi-3d-campus/?to=tech-lab) |
| **樂活圖書館** | 綜合大樓 2F | [👉 導航到樂活圖書館 (`?to=library`)](https://coolokey.github.io/daxi-3d-campus/?to=library) |
