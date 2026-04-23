<div style="max-width: 800px; margin: 40px auto; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; color: #24292e; line-height: 1.6;">
    
    <div style="background: #fff; padding: 40px; border-radius: 16px; border: 1px solid #e1e4e8; box-shadow: 0 12px 24px rgba(0,0,0,0.05);">
        
        <header style="margin-bottom: 35px; border-bottom: 2px solid #f6f8fa; padding-bottom: 20px;">
            <h1 style="font-size: 32px; color: #1b1f23; margin: 0 0 10px 0;">🚀 自動化測試轉型：Selenium 遷移至 Playwright</h1>
            <div style="display: flex; gap: 10px; flex-wrap: wrap;">
                <span style="background: #e7f3ff; color: #0366d6; padding: 4px 12px; border-radius: 20px; font-size: 12px; font-weight: 600;">C# .NET 8</span>
                <span style="background: #e7f3ff; color: #0366d6; padding: 4px 12px; border-radius: 20px; font-size: 12px; font-weight: 600;">Playwright</span>
                <span style="background: #e7f3ff; color: #0366d6; padding: 4px 12px; border-radius: 20px; font-size: 12px; font-weight: 600;">NUnit</span>
            </div>
        </header>

        <section style="margin-bottom: 30px;">
            <h2 style="font-size: 20px; color: #24292e; border-left: 4px solid #0366d6; padding-left: 12px; margin-bottom: 15px;">專案背景 (Situation)</h2>
            <p style="margin: 0; color: #586069;">原有系統採用 Selenium 框架，隨專案規模成長面臨執行效率與穩定性瓶頸：</p>
            <ul style="padding-left: 20px; color: #444;">
                <li style="margin-bottom: 8px;"><strong>效能瓶頸：</strong> 缺乏原生並行支援，測試套件運行時長過大。</li>
                <li style="margin-bottom: 8px;"><strong>穩定性挑戰：</strong> 動態加載導致大量的 Flaky Tests，維護成本極高。</li>
                <li style="margin-bottom: 8px;"><strong>技術限制：</strong> 對現代網頁特性（如 Shadow DOM）支援度較低。</li>
            </ul>
        </section>

        <section style="margin-bottom: 30px;">
            <h2 style="font-size: 20px; color: #24292e; border-left: 4px solid #28a745; padding-left: 12px; margin-bottom: 15px;">執行行動 (Action)</h2>
            <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; border: 1px solid #f1f3f5;">
                <ul style="padding-left: 20px; margin: 0; color: #444;">
                    <li style="margin-bottom: 12px;"><strong>技術 POC 評估：</strong> 針對自動等待機制與執行速度進行對比測試，驗證 Playwright 之優勢。</li>
                    <li style="margin-bottom: 12px;"><strong>架構重新封裝：</strong> 採用 <strong>Page Object Model (POM)</strong> 重構測試邏輯，並統一跨瀏覽器驅動初始化。</li>
                    <li style="margin-bottom: 12px;"><strong>穩定性優化：</strong> 導入 Playwright <b>Auto-waiting</b> 特性，徹底解決非同步等待失效問題。</li>
                    <li style="margin-bottom: 12px;"><strong>環境配置隔離：</strong> 實作動態環境配置管理，支援多環境（Dev/Staging）無縫切換。</li>
                </ul>
            </div>
        </section>

        <section style="margin-bottom: 10px;">
            <h2 style="font-size: 20px; color: #24292e; border-left: 4px solid #f1e05a; padding-left: 12px; margin-bottom: 15px;">最終成果 (Result)</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px;">
                <div style="padding: 15px; background: #fff; border: 1px solid #e1e4e8; border-radius: 8px; text-align: center;">
                    <div style="font-size: 24px; font-weight: bold; color: #28a745;">-30%</div>
                    <div style="font-size: 13px; color: #6a737d;">整體測試執行時程</div>
                </div>
                <div style="padding: 15px; background: #fff; border: 1px solid #e1e4e8; border-radius: 8px; text-align: center;">
                    <div style="font-size: 24px; font-weight: bold; color: #28a745;">-50%</div>
                    <div style="font-size: 13px; color: #6a737d;">錯誤定位調試時間</div>
                </div>
                <div style="padding: 15px; background: #fff; border: 1px solid #e1e4e8; border-radius: 8px; text-align: center;">
                    <div style="font-size: 24px; font-weight: bold; color: #28a745;">High</div>
                    <div style="font-size: 13px; color: #6a737d;">測試穩定度與成功率</div>
                </div>
            </div>
        </section>

        <footer style="margin-top: 40px; padding-top: 20px; border-top: 1px solid #f6f8fa; text-align: right;">
            <span style="color: #6a737d; font-size: 13px;">Tools: Playwright Inspector, Trace Viewer, GitHub Actions</span>
        </footer>
        
      <a href="./" style="display: inline-flex; align-items: center; padding: 8px 16px; background: #f6f8fa; color: #0366d6; text-decoration: none; border-radius: 6px;         font-size: 14px; font-weight: 600; border: 1px solid #e1e4e8; margin-bottom: 30px; transition: 0.2s;">
            ⬅️ 返回首頁
     </a>
    </div>
</div>
