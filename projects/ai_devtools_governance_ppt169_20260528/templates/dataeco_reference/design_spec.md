# dataeco_template — Design Spec

> Example-style workspace for reconstructing the existing DataEco PPT template into a reusable ppt169 deck project. Execution truth for colors, typography, and layout routing lives in `spec_lock.md`.

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | dataeco_template |
| **Canvas Format** | PPT 16:9 (1280×720) |
| **Design Style** | Office-derived minimalist business template |
| **Target Audience** | DataEco internal proposal, report, and client-facing presentation authors |
| **Use Case** | Template reconstruction workspace based on an existing branded PPTX |
| **Created Date** | 2026-05-26 |
| **Source PPTX** | projects/2026 DataEco PPT Template 簡約版.pptx |
| **Template Kind** | deck |
| **Replication Mode** | standard |

---

## II. Source Template Snapshot

- Source theme is the default Office color and type system adapted for DataEco use.
- Known layout set includes cover, title-and-content, section title, comparison, image-caption, and blank variants.
- Existing repo metadata already identifies usable routing for cover, centered title, content, comparison, and story-card scenarios.
- This workspace is intended to preserve brand identity while rebuilding the template into a cleaner, project-style folder structure.

---

## III. Locked Visual Theme

| Role | Value | Note |
| ---- | ----- | ---- |
| **Primary** | `#4472C4` | Accent 1 / main brand blue |
| **Secondary** | `#44546A` | Office dark secondary |
| **Text** | `#000000` | Primary text |
| **Background** | `#FFFFFF` | Default page background |
| **Title Font** | `Calibri Light` | Major font |
| **Body Font** | `Calibri` | Minor font |

---

## IV. Initial Layout Routing

| Content Type | Preferred Layout |
| ------------ | ---------------- |
| Cover / title slide | title_cover |
| Section divider / closing / quote | title_centered |
| Standard content | content_with_image |
| Text-only content | content_centered |
| Comparison | comparison |
| Story card / image caption | story_card |
| Unknown fallback | fallback |

---

## V. Workspace Plan

1. Archive the original PPTX under `sources/` and generate a markdown transcription for structure reference.
2. Import the PPTX into `templates/reference_import/` for manifest, assets, and SVG reference output.
3. Use the imported reference set to derive reconstructed SVG template pages in `svg_output/`.
4. Finalize approved pages into `svg_final/`, then export the rebuilt deck into `exports/`.

---

## VI. Reference Page Roster

### Naming Convention

- `P##_cover_*`: cover variants
- `P##_toc_*`: table-of-contents, agenda, and navigational pages
- `P##_chapter_*`: high-impact section openers or chapter-style visual dividers
- `P##_content_*`: reusable content pages, including charts, maps, frameworks, and brand-guideline pages
- `P##_ending_*`: closing / thank-you pages

### Roster Summary

| Family | Count | Notes |
| ------ | ----- | ----- |
| **Cover** | 2 | Brand-first title pages |
| **TOC** | 5 | Contents, agenda, and map-navigation pages |
| **Chapter** | 7 | Photo-led dividers plus two gradient section pages |
| **Content** | 39 | All reusable business-content, brand-guideline, and asset-library pages |
| **Ending** | 2 | Thank-you closers |

Full per-page mapping is maintained in `notes/01_page_roster.md` and mirrored by the semantic filenames now present in `svg_output/`.
