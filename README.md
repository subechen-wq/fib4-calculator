# FIB-4 Calculator & Clinical Decision Support Tool
### 肝纖維化臨床輔助計算器 (114.06 健保給付修訂版)

[點此開啟工具](https://subechen-wq.github.io/fib4-calculator/)

## 📌 專案背景與目的
在醫院臨床環境中，醫事人員常面臨嚴格的 IT 限制以及複雜的健保藥品給付規範。本專案提供一個 **「零安裝、跨平台、即時反應」** 的工具，協助醫師快速計算 FIB-4 分數，並根據最新規定進行判定。

## 🚀 核心功能
* **即時動態計算**：輸入數值時即刻更新結果，無需額外點擊。
* **視覺化風險分級**：自動對應 **F0 - F4** 分級，並以顏色強化警示。
* [cite_start]**結合健保給付B肝用藥規範**：整合 **114.06.01 生效之 B型肝炎藥品給付規定** 。

## 🩺 臨床邏輯與法規依據

### 1. FIB-4 計算公式
```text
FIB-4 = (Age × AST) / (Platelet × √ALT)

肝纖維化分級切點 (Fibrosis Stage)
F4 ：≧ 6.5
F3 ：≧ 3.25   
F2 ：≧ 2.1   
F1 ：≧ 1.3
F0 ：< 1.3

114.06.01 健保給付門檻提醒   
符合 F3 條件：FIB-4 ≧ 3.25。適用於 HBeAg(+) 患者，ALT ≧ 正常值上限且半年內有兩次以上紀錄（間隔 ≧ 3 個月）。  
符合 F2 條件：FIB-4 ≧ 2.1。適用於 HBeAg(-) 患者，需配合 HBV DNA ≧ 2000 IU/mL 且 ALT 符合規範者 。

🛠️ 技術棧 (Tech Stack)
Frontend: HTML5, CSS3, JavaScript (Vanilla JS)
Deployment: GitHub Pages
Integration: LINE Front-end Framework (LIFF)

⚖️ 免責聲明
本工具僅供醫療專業人員參考，計算結果不可取代醫師之專業臨床判斷。
