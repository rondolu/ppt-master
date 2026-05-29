# Execution Lock

## canvas

- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors

- bg: #FFFFFF
- text: #000000
- primary: #4472C4
- secondary: #44546A
- accent_2: #ED7D31
- accent_3: #A5A5A5
- accent_4: #FFC000
- accent_5: #5B9BD5
- accent_6: #70AD47
- link: #0563C1
- visited_link: #954F72

## typography

- title_family: Calibri Light, Arial, sans-serif
- body_family: Calibri, Arial, sans-serif
- emphasis_family: Calibri Light, Arial, sans-serif
- body: 20
- title: 30
- subtitle: 22
- annotation: 12
- footnote: 10

## layouts

- title_cover: layout 0 | 標題投影片
- content_centered: layout 1 | 標題及內容
- title_centered: layout 2 | 章節標題
- column_2: layout 3 | 兩個內容
- comparison: layout 4 | 比較
- title_only: layout 5 | 只有標題
- blank: layout 6 | 空白
- content_with_image: layout 7 | 含輔助字幕的內容
- story_card: layout 8 | 含輔助字幕的圖片
- title_vertical: layout 9 | 標題及直排文字
- master_base: layout 10 | 直排標題及文字

## routing

- title_slide: title_cover
- section_divider: title_centered
- closing: title_centered
- thank_you: title_centered
- quote: title_centered
- content: content_with_image
- content_no_image: content_centered
- comparison: comparison
- framework_2col: column_2
- story_card: story_card
- fallback: title_centered

## forbidden

- Changing the locked Office-derived palette before template reconstruction is reviewed
- Mixing unrelated font families into the base template
- Using non-ppt169 canvas sizes in reconstructed SVG pages
