# Slide 1: AI 輔助開發效率優化

## AI 輔助開發效率優化：GitHub 萬星提示詞專案架構解析

### Andrej Karpathy 實務觀察與解決方案

前 Tesla AI 總監暨 OpenAI 聯合創始人
2026年

---

# Slide 2: 問題背景

**Visual: hero-statement**

AI 程式碼生成工具普遍存在三大缺陷，導致開發效率大幅降低

---

# Slide 3: 三大核心缺陷

**Visual: content_no_image**

**Karpathy 指出的三大 AI 開發工具缺陷**

- {bold}假設先驗 (Blind Assumptions){/bold}：面臨模糊需求時缺乏澄清機制，徑自執行導致方向偏差
- {bold}過度設計 (Over-engineering){/bold}：將簡單問題複雜化，引入非必要設計模式與架構層次
- {bold}附帶修改 (Collateral Damage){/bold}：局部修改引發非預期改動，破壞既有架構風格

---

# Slide 4: 三大缺陷詳析

**Visual: comparison-2**

[Column 1: 假設先驗 vs 過度設計]
- 缺乏主動詢問機制，預設執行路徑
- 耗費大量時間修正方向性錯誤
- 引入非必要 Design Patterns 與 Interfaces
- 程式碼體積膨脹，維護成本高

[Column 2: 附帶修改的代價]
- 修復函式時連帶更改縮排與註解
- 破壞既有架構，難以追溯
- Code Review 困難度大幅提升
- 開發流程受阻，效率損耗嚴重

---

# Slide 5: 解決方案

**Visual: bullets**

**開源社群回應：系統提示詞輕量化解決方案**

- 基於 {bold}系統提示詞 (System Prompts){/bold} 的輕量級約束框架
- 單月於 GitHub 累計逾 {bold}12 萬顆星{/bold}，獲廣泛社群驗證
- 相容 Claude Code、Cursor 等主流 AI 開發環境
- 無需安裝依賴套件，提示詞設定檔置於專案根目錄即可生效
- 將 AI 從被動執行者重塑為{blue}具備邊界意識的協作模組{/blue}

---

# Slide 6: 四大系統化約束原則

**Visual: comparison-2**

[Column 1: 行為約束]
- {signpost}原則一{/signpost} 強制事前評估 (Think Before Coding)
- 禁止未確認前執行假設
- 需求模糊時強制暫停並提出選項
- {signpost}原則二{/signpost} 防範過度設計 (No Over-engineering)
- 程式碼嚴格對齊當前需求範圍
- 禁止預留未來擴充性之複雜設計

[Column 2: 執行紀律]
- {signpost}原則三{/signpost} 標靶式修改 (Targeted Modifications)
- 僅修改具直接相依性之程式碼片段
- 無條件繼承專案既有編碼風格
- {signpost}原則四{/signpost} 結果導向驗收 (Outcome-based Execution)
- 著重定義驗收標準而非實作步驟
- 先建立可重現測試，再進行程式碼修正

---

# Slide 7: 原則一與原則二

**Visual: comparison-2**

[Column 1: 強制事前評估]
- 禁止 AI 在未確認下執行任何預設假設
- 需求具歧義時，系統必須暫停提問
- 建立「需求雙向確認」機制
- 以初始溝通成本換取後續重構節省

[Column 2: 防範過度設計]
- 生成程式碼必須嚴格對齊當前需求
- 禁止導入非必要設計模式與介面
- 禁止為「未來擴充性」預留架構
- 通過資深工程師「適度設計」標準審查

---

# Slide 8: 原則三與原則四

**Visual: comparison-2**

[Column 1: 標靶式修改]
- 僅修改與任務具直接相依性之程式碼
- 明文禁止縮排調整與無關模組重構
- 禁止擅自修改現有註解
- 無條件繼承並遵循既有 Coding Style

[Column 2: 結果導向驗收]
- 指令著重定義「驗收標準 (What)」
- 非詳述「實作步驟 (How)」
- 範例：先建立重現缺陷之單元測試，再修正直至通過
- 賦予 LLM 於明確邊界內自主迭代能力

---

# Slide 9: 部署與整合實務

**Visual: comparison-2**

[Column 1: 支援環境]
- {bold}Claude Code{/bold}
- {bold}Cursor{/bold}
- 具 .cursorrules 讀取權限之 AI 輔助開發環境
- 支援專案層級指令檔案讀取

[Column 2: 部署門檻極低]
- 無需安裝任何額外依賴套件
- 無需撰寫控制邏輯
- 提示詞設定檔置於專案根目錄
- AI 助理初始化階段自動掛載約束集

---

# Slide 10: 專業洞察

> 「在諸多情境下，最具價值的工程實踐並非創造嶄新的基礎設施，而是將已獲共識之核心原則，以最低的使用門檻普及化。」

---

# Slide 11: 結語

**Visual: hero-statement**

解決 AI 開發挑戰的關鍵，在於重新確立精確的人機互動指令邊界

---
