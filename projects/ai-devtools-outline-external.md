<!-- markdownlint-disable MD025 MD036 MD032 -->

# Slide 1: AI 輔助開發治理

## AI 輔助開發治理

### 從 GitHub 萬星提示詞專案看協作邊界設計

An operational view inspired by Andrej Karpathy
2026年

---

# Slide 2: 為什麼值得關注

**Visual: hero-statement**

當 AI 開始參與程式開發，真正決定效率與品質的，是協作規則是否足夠精確

---

# Slide 3: 目前最常見的三個失效點

**Visual: bullets**

**Karpathy 指出的三大風險，會直接拉高開發與審查成本**

- {bold}假設先驗{/bold}：需求有歧義時不先澄清，直接選路徑執行
- {bold}過度設計{/bold}：替簡單任務引入過多架構、介面與抽象層
- {bold}附帶修改{/bold}：修一處卻動到無關模組、縮排與註解風格
- 三者共同結果是 {blue}方向偏差、維護膨脹、審查變慢{/blue}

---

# Slide 4: 問題的管理成本

**Visual: comparison-2**

[Column 1: 對團隊的直接影響]
- 工程師要花時間修正 AI 的錯方向
- 程式碼體積變大，閱讀與維護成本上升
- Review 討論被無關變更稀釋
- 專案節奏容易被反覆來回拖慢

[Column 2: 對決策層的訊號]
- 這不是單點 bug，而是流程治理問題
- 缺乏約束會放大模型的不穩定性
- 工具越普及，治理成本越需要前置化
- 管理焦點應從工具導入轉向使用規範

---

# Slide 5: 社群給出的解法

**Visual: content_no_image**

**用一組低成本、可複製的提示詞約束，把 AI 從被動執行者變成可治理的協作模組**

- 核心做法是把邊界、停損點與驗收方式寫進系統提示詞
- 這類專案已在 GitHub 快速累積高關注度，顯示需求具有普遍性
- 優勢在於導入門檻低，不需要改模型或額外建構複雜基礎設施

---

# Slide 6: 四大約束原則

**Visual: comparison-2**

[Column 1: 設計原則]
- {signpost}Think Before Coding{/signpost} 需求未清楚前先停下來確認
- {signpost}No Over-engineering{/signpost} 只做當下需要的解法
- {signpost}Targeted Modifications{/signpost} 只改與任務直接相關的程式碼
- {signpost}Outcome-based Execution{/signpost} 以驗收標準驅動修正流程

[Column 2: 可落地的管理要求]
- 模糊需求必須先澄清，不允許自動假設
- 禁止預先為未來擴充性堆疊過多架構
- 禁止局部修復時順手重構無關區塊
- 優先要求可驗證結果，例如先補測試再修正

---

# Slide 7: 結語

**Visual: hero-statement**

真正可規模化的 AI 開發能力，來自明確規則、可驗證結果，以及對修改邊界的共同紀律

---
