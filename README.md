# FIB-4 Calculator & Clinical Decision Support Tool
### 肝纖維化臨床輔助計算器 (114.06 健保給付修訂版)

[點此開啟工具](https://subechen-wq.github.io/fib4-calculator/)

## 🌐 Deployment & Integration

本工具已正式部署並整合 **LINE LIFF (LINE Front-end Framework)** 技術，確保醫事人員於門診或巡房時，可透過行動裝置進行無縫操作。

* [cite_start]**即時決策支援**：針對 **114.06.01 生效之 HBV 藥品給付規定** 實施 ，提供臨床醫師最即時的藥品給付門檻判定支援。
* **行動端體驗**：透過 LINE 介面即可快速開啟，解決醫院內部電腦對外部網頁存取的 IT 限制。
* **專屬連結**：[點此由 LINE 開啟計算器](您的LIFF網址)

## 📌 專案背景與目的
在醫院臨床環境中，醫事人員常面臨嚴格的 IT 限制以及複雜的健保藥品給付規範。本專案提供一個 **「零安裝、跨平台、即時反應」** 的工具，協助醫師快速計算 FIB-4 分數，並根據最新規定進行判定。

## 🚀 核心功能
* **即時動態計算**：輸入數值時即刻更新結果，無需額外點擊。
* **視覺化風險分級**：自動對應 **F0 - F4** 分級，並以顏色強化警示。
* [cite_start]**結合健保給付B肝用藥規範**：整合 **114.06.01 生效之 B型肝炎藥品給付規定** 。

## 🛠️技術棧 (Tech Stack)
* Frontend: HTML5, CSS3, JavaScript (Vanilla JS)
* Deployment: GitHub Pages
* Integration: LINE Front-end Framework (LIFF)

## ⚖️免責聲明 
本工具僅供醫療專業人員參考，計算結果不可取代醫師之專業臨床判斷。

## 🩺 臨床邏輯與法規依據
* **114.06.01健保給付門檻提醒** 
符合 F3條件: HBeAg(+) 患者給付門檻：ALT > X (半年內兩次以上，間隔大於 3 個月)且HBV DNA ≧ 20000 IU/mL。。  
符合 F2條件: HBeAg(-) 患者給付門檻：ALT > X (半年內兩次以上，間隔大於 3 個月)且HBV DNA ≧ 20000 IU/mL 。

### 1. FIB-4 計算公式
```text
FIB-4 = (Age × AST) / (Platelet × √ALT)

肝纖維化分級切點 (Fibrosis Stage)
F4 ：≧ 6.5
F3 ：≧ 3.25   
F2 ：≧ 2.1  
F1 ：≧ 1.3
F0 ：< 1.3

