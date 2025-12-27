# iOS SwiftUI Calculator with Currency Converter

這是一個使用 SwiftUI 開發的 iOS 計算機應用程式。除了具備標準計算機的基本運算功能外，還整合了即時匯率換算功能，讓使用者能在計算的同時進行貨幣轉換。

## 📱 介面展示 (Demo)

<p align="center">
  <img src="calculator_screen.gif" alt="Login & Home" width="300" />
</p>

---

## ✨ 功能特色 (Features)

* **基本運算**：支援加 (`+`)、減 (`-`)、乘 (`×`)、除 (`÷`) 四則運算。
* **進階功能**：包含百分比 (`%`) 計算與正負號切換 (`+/-`)。
* **多國貨幣換算**：
    * 支援 **台幣 (TWD)**、**美金 (USD)**、**日圓 (JPY)** 之間的即時金額轉換。
    * 透過選單 (ActionSheet) 快速切換當前幣別。
    * *註：匯率目前為固定值 (1 USD = 30 TWD, 1 JPY = 0.27 TWD)。*
* **現代化 UI**：採用類似原生 iOS 計算機的圓形按鈕設計，並使用 SwiftUI 建構響應式介面。

## 🛠 技術規格 (Tech Stack)

* **語言**：Swift 5.0
* **框架**：SwiftUI
* **開發工具**：Xcode 16.0+
* **目標版本**：iOS 18.0+

## 🚀 安裝與執行 (Installation)

1. **Clone 專案**
   ```bash
   git clone [https://github.com/your-username/calculator.git](https://github.com/your-username/calculator.git)
   ```
2. **開啟專案** 使用 Xcode 開啟 `calculator.xcodeproj` 檔案。
3. **執行**
   選擇模擬器或實體裝置（需 iOS 18.0 以上），按下 `Cmd + R` 即可執行。

## 📂 專案結構 (File Structure)

* `calculatorApp.swift`：應用程式的進入點 (Entry Point)，負責啟動 App 並載入主畫面。
* `ContentView.swift`：主要的 UI 佈局與邏輯核心。
    * **UI 佈局**：使用 `VStack` 與 `HStack` 排列顯示螢幕與按鈕矩陣。
    * **核心變數**：
        * `display`：控制螢幕上顯示的數字字串。
        * `selectedCurrency`：追蹤當前選擇的貨幣單位 (TWD/USD/JPY)。
    * **關鍵函式**：
        * `buttonTapped(_:)`：處理數字與運算符號的輸入邏輯。
        * `calculateResult()`：執行加減乘除的實際運算。
        * `convertCurrency(to:)`：負責處理不同幣別間的匯率換算邏輯。

---

## 👤 作者 (Author)

* **Name**: 楊浤立
* **Student ID**: 01157025
* **Created Date**: 2024/11/28
* **Medium Blog**: [點擊閱讀開發心得](https://medium.com/%E6%B5%B7%E5%A4%A7-ios-app-%E7%A8%8B%E5%BC%8F%E8%A8%AD%E8%A8%88/ios%E6%87%89%E7%94%A8%E7%A8%8B%E5%BC%8F%E9%96%8B%E7%99%BC%E5%85%A5%E9%96%80-%E5%8A%A0%E5%88%86%E4%BD%9C%E6%A5%AD-calculator-%E5%8C%AF%E7%8E%87%E6%8F%9B%E7%AE%97%E7%9A%84%E5%9F%BA%E6%9C%AC%E5%8A%9F%E8%83%BD-2ee642b3fcc6) ✍️
   
