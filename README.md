# 🏠 新北市預售屋實價登錄查詢系統

> 資料來源：內政部不動產實價登錄 | 共 44,979 筆預售屋交易資料

## 🌐 系統網址

部署完成後填入：`（Azure 部署後更新此處）`

---

## 📁 檔案說明

| 檔案 | 說明 |
|------|------|
| `index.html` | 主頁面（整合三個功能） |
| `widget-1-search.html` | 搜尋篩選 + 資料清單 |
| `widget-2-charts.html` | 統計圖表分析 |
| `widget-3-calculator.html` | 價格計算器 |
| `data.json` | 所有交易資料（44,979 筆，~11MB） |
| `staticwebapp.config.json` | Azure Static Web Apps 設定檔 |

---

## ☁️ Azure Static Web Apps 部署步驟

### 1. 登入 Azure Portal
前往 [portal.azure.com](https://portal.azure.com) 並登入

### 2. 建立 Static Web App
- 搜尋 **Static Web Apps** → 點「建立」
- 填寫設定：
  - 方案類型：**免費**
  - 區域：**East Asia**
  - 部署來源：**GitHub**

### 3. 連接此 GitHub Repo
- 組織：`ellen3149-mogo`
- 存放庫：`HYML`
- 分支：`main`
- 應用程式位置：`/`

### 4. 完成部署
建立完成後約 2-3 分鐘，Azure 會自動從此 repo 拉取檔案並部署。

---

## 🔗 嵌入 Google Sites

取得 Azure 網址後，在 Google Sites：
- 插入 → 嵌入 → **網址** → 貼上 Azure 網址

---

## 功能說明

| 功能 | 說明 |
|------|------|
| 🔍 搜尋篩選 | 依行政區、建物型態、格局、總價、單價等多條件篩選，支援排序與分頁 |
| 📊 統計分析 | 各區均價長條圖、成交量圓餅圖、建物型態分布、總價區間分布 |
| 🧮 價格計算 | 由單價算總價、由總價反推單價，含房貸試算與負擔率分析 |
