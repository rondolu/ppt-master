<!-- markdownlint-disable MD022 MD032 MD033 MD041 -->

## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- bg: #FFFFFF
- secondary_bg: #F4FBF8
- surface: #F3F3F3
- primary: #00AA64
- primary_dark: #009056
- primary_soft: #3BBB8E
- node_soft: #6EDAA8
- gradient_start: #C3FFC0
- gradient_mid: #8CECBD
- accent: #2BCB8A
- secondary_accent: #9AE992
- accent_lime: #F3FC78
- accent_mint: #86E8B9
- overlay_dark: #0F172A
- sidebar_top: #8DECC1
- sidebar_mid: #A7F3D0
- sidebar_soft: #C8F9D9
- sidebar_glow: #6EE7B7
- text: #111827
- text_secondary: #4B5563
- text_muted: #808080
- connector: #AFABAB
- border: #D9D9D9
- success: #00AA64
- warning: #D97706

## typography
- font_family: Microsoft JhengHei, Arial, sans-serif
- title_family: Microsoft JhengHei, Arial, sans-serif
- body_family: Microsoft JhengHei, Arial, sans-serif
- emphasis_family: Arial, "Microsoft JhengHei", sans-serif
- label_family: Arial, sans-serif
- code_family: Consolas, "Courier New", monospace
- body: 20
- title: 34
- subtitle: 24
- annotation: 12
- footnote: 10
- cover_title: 56
- hero_title: 42
- title_l2: 32
- title_l3: 28
- body_small: 16

## gradients
- brand_band: #C3FFC0 -> #3BBB8E
- brand_core: #009056 -> #00AA64 -> #9AE992
- brand_signal: #3BBB8E -> #86E8B9 -> #F3FC78

## icons
- library: chunk-filled
- motif: solid icons placed in circular or rounded gradient chips inspired by the DataEco icon guide pages
- inventory: shield, target-arrow, users, chart-bar, circle-checkmark, triangle-exclamation, cloud, magnifier, calendar, sitemap

## images
- cover_bg: templates/images/reference_import_assets/image1.png
- quote_bg: templates/images/reference_import_assets/image6.png
- content_canvas: templates/images/reference_import_assets/image20.png | no-crop
- closing_bg: templates/images/reference_import_assets/image86.png

## design_references
- connector_page: templates/dataeco_reference/P43_content_connector_diagram.svg
- palette_page: templates/dataeco_reference/P44_content_color_palette_spec.svg
- color_usage_page: templates/dataeco_reference/P45_content_color_usage_guide.svg
- gradient_page: templates/dataeco_reference/P46_content_gradient_palette.svg
- typography_zh_page: templates/dataeco_reference/P47_content_typography_chinese.svg
- typography_en_page: templates/dataeco_reference/P48_content_typography_english.svg
- icon_page: templates/dataeco_reference/P50_content_icon_library_grid.svg
- gradient_icon_page: templates/dataeco_reference/P51_content_gradient_icon_library.svg
- section_divider_page: templates/dataeco_reference/P52_chapter_gradient_content_a.svg

## page_rhythm
- P01: anchor
- P02: breathing
- P03: dense
- P04: dense
- P05: breathing
- P06: dense
- P07: anchor

## page_layouts
- P01: P01_cover_brand_hero
- P02: P07_content_quote_photo
- P03: P43_content_connector_diagram
- P04: P18_content_comparison_three_columns
- P05: P17_content_process_four_steps
- P06: P43_content_connector_diagram
- P07: P54_ending_thank_you_a

## forbidden
- Mixing icon libraries
- Introducing colors outside the locked DataEco palette and gradients without a clear content reason
- Reverting analytical pages to flat generic cards when connector relationships should carry the meaning
- rgba()
- <style>, class, <foreignObject>, textPath, @font-face, <animate*>, <script>, <iframe>, <symbol>+<use>
- <g opacity>
- HTML named entities in text
