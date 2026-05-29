# ai_devtools_governance - Design Spec

> Human-readable design narrative for a 7-page governance deck built from the AI development outline and restyled with the DataEco element-guide pages under templates/dataeco_reference as the primary visual reference.

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | ai_devtools_governance |
| **Canvas Format** | PPT 16:9 (1280×720) |
| **Page Count** | 7 |
| **Design Style** | DataEco brand-guide-informed corporate governance style |
| **Target Audience** | 技術主管、工程團隊 lead、AI 導入決策者 |
| **Use Case** | 內部治理簡報、AI 協作規範分享、管理層對齊會議 |
| **Created Date** | 2026-05-28 |

---

## II. Canvas Specification

| Property | Value |
| -------- | ----- |
| **Format** | PPT 16:9 |
| **Dimensions** | 1280×720 |
| **viewBox** | `0 0 1280 720` |
| **Margins** | left/right 72px, top 64px, bottom 44px |
| **Content Area** | Main content inside x=108~1200, y=92~650; left sidebar/background chrome reserved for template identity and section signaling |

---

## III. Visual Theme

### Theme Style

- **Style**: DataEco corporate governance deck rebuilt from the template's connector, palette, gradient, typography, and icon guide pages
- **Theme**: Light theme
- **Tone**: professional, disciplined, system-oriented, clean

### Color Scheme

| Role | HEX | Purpose |
| ---- | --- | ------- |
| **Background** | `#FFFFFF` | Main slide background |
| **Secondary bg** | `#F4FBF8` | Card fill, takeaway strip, light emphasis |
| **Primary** | `#00AA64` | Template brand green, active relationship lines, section markers |
| **Primary dark** | `#009056` | Strong callouts, terminal nodes, highlighted outcomes |
| **Primary soft** | `#3BBB8E` | Pills, chips, soft emphasis modules |
| **Accent** | `#2BCB8A` | Secondary highlight, dividers, emphasis chips |
| **Secondary accent** | `#9AE992` | Connector highlight and soft gradient tail |
| **Accent lime** | `#F3FC78` | Bright signal accent for terminal emphasis |
| **Accent mint** | `#86E8B9` | Gradient transition tone |
| **Body text** | `#111827` | Main body copy |
| **Secondary text** | `#4B5563` | Supporting text |
| **Muted text** | `#808080` | Secondary captions and guide labels |
| **Connector gray** | `#AFABAB` | Dashed neutral relationship lines |
| **Border/divider** | `#D9D9D9` | Card borders and separators |
| **Surface** | `#F3F3F3` | Neutral chip and guide surface |
| **Success** | `#00AA64` | Positive emphasis |
| **Warning** | `#D97706` | Risk or caution emphasis |

### Gradient Scheme

```xml
<linearGradient id="brandBand" x1="0%" y1="0%" x2="100%" y2="100%">
  <stop offset="0%" stop-color="#C3FFC0"/>
  <stop offset="96%" stop-color="#3BBB8E"/>
</linearGradient>

<linearGradient id="brandCore" x1="0%" y1="0%" x2="100%" y2="100%">
  <stop offset="0%" stop-color="#009056"/>
  <stop offset="34%" stop-color="#00AA64"/>
  <stop offset="100%" stop-color="#9AE992"/>
</linearGradient>

<linearGradient id="brandSignal" x1="100%" y1="100%" x2="0%" y2="0%">
  <stop offset="0%" stop-color="#F3FC78"/>
  <stop offset="43%" stop-color="#8CECBD"/>
  <stop offset="100%" stop-color="#3BBB8E"/>
</radialGradient>
```

These three gradients are taken directly from the DataEco gradient guide logic and reused for headline bands, chips, and emphasis nodes instead of introducing ad-hoc fills.

---

## IV. Typography System

### Font Plan

**Typography direction**: Use the template typography guide literally. Chinese text follows the dedicated Chinese font page, while English labels and numerals follow the English typography page.

| Role | Chinese | English | Fallback tail |
| ---- | ------- | ------- | ------------- |
| **Title** | `Microsoft JhengHei Bold` | `Arial Bold` | `Arial, sans-serif` |
| **Body** | `Microsoft JhengHei` | `Arial` | `Arial, sans-serif` |
| **Emphasis** | `Microsoft JhengHei Bold` | `Arial Bold` | `Arial, sans-serif` |
| **Code** | — | `Consolas, Courier New` | `monospace` |

**Per-role font stacks**:

- Title: `Microsoft JhengHei, Arial, sans-serif`
- Body: `Microsoft JhengHei, Arial, sans-serif`
- Emphasis: `Arial, Microsoft JhengHei, sans-serif`
- Code: `Consolas, "Courier New", monospace`

### Font Size Hierarchy

**Baseline**: Body font size = 20px

| Purpose | Ratio to body | Recommended size | Weight |
| ------- | ------------- | ---------------- | ------ |
| Cover title | 2.5-3x | 52-56px | Bold |
| Section / hero statement | 1.8-2.3x | 36-42px | Bold |
| Page title | 1.5-1.8x | 30-34px | Bold |
| Subtitle | 1.1-1.3x | 22-24px | SemiBold |
| **Body content** | **1x** | **20px** | Regular |
| Body secondary | 0.8x | 16px | Regular |
| Annotation / caption | 0.6-0.75x | 12-15px | Regular |
| Page number / footer | 0.5-0.65x | 10-13px | Regular |

The Chinese guide pages also establish the effective hierarchy used in this deck: 36pt / 25pt / 22pt / 18pt / 14pt / 12pt equivalents, mapped into the SVG pixel system above.

### Formula Rendering Policy

- **Policy**: text-only
- **Rationale**: This governance deck contains no formula-worthy expressions; all text remains editable.

---

## V. Layout Principles

### Page Structure

- **Header area**: 56-76px title zone aligned to the content column, often paired with a takeaway strip, section chip, or connector legend.
- **Content area**: Main analytical body using connector-led flows, two-column governance comparisons, relationship chips, or single-statement hero layouts.
- **Footer area**: Small source/context line or simple page marker when needed; chrome remains visually light.

### Layout Pattern Library

| Pattern | Suitable Scenarios |
| ------- | ----------------- |
| **Full-bleed cover** | Opening and closing anchor pages |
| **Hero statement over image** | Slide 2 narrative pause and emphasis |
| **Connector-linked analysis map** | Slide 3 failure-point decomposition and Slide 6 principle-to-requirement mapping |
| **Two-column comparison with central control band** | Slide 4 side-by-side management framing |
| **Process flow with gradient stages** | Slide 5 solution explanation |

### Spacing Specification

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Safe margin from canvas edge | 40-72px | 72px |
| Content block gap | 24-36px | 28px |
| Card gap | 20-30px | 24px |
| Card padding | 18-26px | 22px |
| Card radius | 14-18px | 16px |
| Connector dash rhythm | 4px dash / 4px gap | 4/4 |
| Chip radius | 4-11px | mixed by emphasis level |

---

## VI. Icon Usage Specification

### Source

- **Built-in icon library**: `chunk-filled`
- **Usage method**: SVG placeholder `<use data-icon="chunk-filled/...">`, usually nested inside circular or rounded gradient chips inspired by the DataEco icon guide pages

### Recommended Icon List

| Purpose | Icon Path | Page |
| ------- | --------- | ---- |
| Governance guardrail | `chunk-filled/shield` | P03, P06 |
| Target / operating principle | `chunk-filled/target-arrow` | P05 |
| Collaboration | `chunk-filled/users` | P04 |
| Review / validation | `chunk-filled/circle-checkmark` | P06 |
| Risk | `chunk-filled/triangle-exclamation` | P03 |
| Data / analysis | `chunk-filled/chart-bar` | P04 |
| Search / diagnosis | `chunk-filled/magnifier` | P03 |
| Workflow / structure | `chunk-filled/sitemap` | P05, P06 |

---

## VII. Visualization Reference List

- The deck does not use numeric charts, but it does borrow visual language from these template guide pages:
  - `P43_content_connector_diagram.svg` for dashed relationship lines and connector nodes
  - `P44_content_color_palette_spec.svg` and `P45_content_color_usage_guide.svg` for palette discipline
  - `P46_content_gradient_palette.svg` for the three locked gradient families
  - `P47_content_typography_chinese.svg` and `P48_content_typography_english.svg` for the font hierarchy
  - `P50_content_icon_library_grid.svg` and `P51_content_gradient_icon_library.svg` for icon-chip treatment
- There are no numeric charts requiring coordinate calibration.

---

## VIII. Image Resource List

- No external image acquisition is required.
- This deck reuses bundled template assets already staged inside the project:
  - `templates/images/reference_import_assets/image1.png` for the cover
  - `templates/images/reference_import_assets/image6.png` for the hero statement page
  - `templates/images/reference_import_assets/image20.png` as the DataEco content canvas background
  - `templates/images/reference_import_assets/image86.png` for the closing page
- The element-guide SVG pages staged under `templates/dataeco_reference/` are treated as first-class visual references for connectors, palette, gradients, typography, and icon treatment.

---

## IX. Content Outline

| Page | Title | Objective | Content Brief | Rhythm | Layout |
| ---- | ----- | --------- | ------------- | ------ | ------ |
| **P01** | AI 輔助開發治理 | Establish topic and frame | Main title, subtitle, operational framing, year marker | anchor | DataEco brand cover with typography-guide hierarchy |
| **P02** | 為什麼值得關注 | Deliver one hero takeaway | A single sentence stating that collaboration rules determine AI development quality | breathing | Quote / hero statement over image |
| **P03** | 目前最常見的三個失效點 | Break down the three risks | Assumption-first, over-engineering, collateral edits; connected into a shared downstream cost node | dense | Connector-linked risk map |
| **P04** | 問題的管理成本 | Show two-sided management impact | Team-level direct cost vs management-level governance signal, bridged by a shared control band | dense | Two-column comparison with connectors |
| **P05** | 社群給出的解法 | Explain the remedy | Low-cost prompt constraints as governance mechanism; why adoption is rising | breathing | Gradient process flow |
| **P06** | 四大約束原則 | Translate ideas into operating rules | Four design principles paired against four management requirements through connector logic | dense | Connector-based principle matrix |
| **P07** | 真正可規模化的 AI 開發能力 | End on a disciplined closing statement | Hero conclusion on clear rules, verifiable outcomes, and change boundaries | anchor | DataEco ending reference |

---

## X. Speaker Notes Strategy

| Page | Notes Direction |
| ---- | --------------- |
| **P01** | Open with the management lens: AI coding efficiency depends on collaboration boundaries, not only model capability. |
| **P02** | State the core thesis in one sentence and use it to pivot from tooling hype to governance precision. |
| **P03** | Walk through the three failure modes as recurring operating risks, not isolated mistakes. |
| **P04** | Contrast engineer-facing cleanup cost with management-facing governance signals. |
| **P05** | Explain that prompt constraints act as an operational control layer rather than a model upgrade. |
| **P06** | Translate the four principles into enforceable review and execution rules. |
| **P07** | Close by reinforcing that scale comes from shared discipline around rules and validation. |

---

## XI. Technical Constraints

- Reuse the staged DataEco reference assets under `templates/` only; do not introduce new external dependencies.
- Keep all pages at viewBox `0 0 1280 720`.
- Preserve the light, business-first visual system of the DataEco reference deck.
- Use the locked DataEco element-guide pages as the source of truth for connector stroke style, gradient family, typography hierarchy, and icon-chip treatment.
- No AI-generated images, no formula rendering, no chart-calibration workflow required.
- Maintain editable text wherever possible and avoid decorative over-design.
