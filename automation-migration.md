# 🚀 自動化測試轉型：Selenium 遷移至 Playwright 的評估與執行

[⬅️ 返回首頁](./)

## 專案背景 (Situation)
原本系統採用 **Selenium** 作為主要測試框架，但隨著專案規模擴大，面臨以下挑戰：
* **執行速度受限：** 缺乏原生的並行執行支持，測試套件運行時間過長。
* **測試穩定度 (Flaky Tests)：** 頻繁出現非同步加載導致的等待失效，需手動編寫大量的 `Thread.Sleep` 或複雜的顯式等待。
* **現代網頁特性支援不足：** 在處理 Shadow DOM 與複雜彈窗時，Selenium 的定位與操作較為繁瑣。

## 核心任務 (Task)
評估並導入 **Playwright** 框架，目標是建立一套更穩定、更快速且易於維護的 E2E 測試環境，並確保現有的測試案例能平滑遷移。

## 執行行動 (Action)
在遷移過程中，我執行了以下關鍵任務：
* **技術 POC 評估：** 對比 Selenium 與 Playwright 在自動等待機制、執行速度及開發工具 (Codegen/Inspector) 的差異。
* **架構重新封裝：** * 使用 **C# + NUnit** 重新建構 **Page Object Model (POM)**。
    * 統一處理跨瀏覽器（Chromium, Firefox, WebKit）的驅動初始化邏輯。
* **穩定性優化：** 利用 Playwright 的 **Auto-waiting** 特性，移除代碼中不穩定的等待邏輯，顯著降低測試失敗率。
* **環境配置隔離：** 實作動態 `appsettings.json` 管理機制，支援開發、測試與預發布環境的快速切換。

## 最終成果 (Result)
* **執行效率提升：** 透過 Playwright 的並行執行 (Parallelism)，整體測試執行時間**縮短了約 30%**。
* **維護成本降低：** 測試代碼量減少，邏輯更加清晰，新進成員的上手門檻大幅降低。
* **調試效率：** 利用 Playwright 的錄影 (Video) 與 Trace Viewer 功能，使定位錯誤原因的時間減少了 50%。

---

### 🛠 技術棧
* **語言：** C# (.NET 8)
* **框架：** Playwright, NUnit
* **工具：** Playwright Inspector, Trace Viewer

[⬅️ 返回首頁](./)
