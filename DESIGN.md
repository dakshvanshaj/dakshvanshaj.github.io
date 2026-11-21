# Design System

<!-- impeccable:design-tokens -->

## World

Quiet Human Editorial / Restrained Natural Paper

## Principles

1. **No Slop:** No dark sci-fi HUDs, no neon glow, no Inter-everywhere, no nested cards-inside-cards, no unearned decorative gradients.
2. **Tactile Natural Ground:** Warm, paper-like ground (`#F5F2EB`) that provides organic visual warmth and deep reading comfort.
3. **Typographic Authority:** Warm literary editorial serif for headlines (`Newsreader`) paired with an understated, readable grotesque sans (`Plus Jakarta Sans`) and tabular figures for data.
4. **Authentic Artifacts:** Real brand logos (Simple Icons standard), real application captures (18 live Narada OS screenshots), real demo video, and real founder portrait.
5. **Radical Honesty:** Transparent labels and claims. No simulated client adoption. No inflated metrics.

## Color Tokens

- `--bg-ground`: `#F8FAFC` (Clean architectural slate-tinted canvas)
- `--bg-surface`: `#F1F5F9` (Subtle container / panel surface)
- `--bg-card`: `#FFFFFF` (Crisp elevated white card surface)
- `--border-subtle`: `#E2E8F0` (Muted hairline divider)
- `--border-focus`: `#0F172A` (High-contrast focus boundary)
- `--text-primary`: `#0F172A` (Deep slate ink, >13:1 contrast)
- `--text-secondary`: `#334155` (Slate body text, >7:1 contrast)
- `--text-tertiary`: `#475569` (Metadata and secondary labels, >5.5:1 contrast)
- `--accent-terracotta`: `#C2410C` (Warm burnt rust accent)
- `--accent-hover`: `#9A3412`
- `--accent-action`: `#0F172A` (Primary action button surface)
- `--accent-action-text`: `#F8FAFC` (Button label)
- `--selection-bg`: `#E2E8F0`
- `--selection-text`: `#0F172A`

## Typography

- **Display & Headings:** `Newsreader` (optical size 6..72, weights 400, 500)
- **Body & Controls:** `Plus Jakarta Sans`, system-ui, -apple-system, sans-serif (weights 400, 500, 600)
- **Code & Measurements (When real only):** `JetBrains Mono`, monospace (weight 400)
- **Scale:**
  - Hero Headline: 2.25rem (36px) – 2.75rem (44px), line-height 1.25
  - Section Headings: 1.5rem (24px) – 1.875rem (30px), line-height 1.3
  - Project Titles: 1.25rem (20px) – 1.375rem (22px), line-height 1.35
  - Body Text: 0.9375rem (15px) – 1rem (16px), line-height 1.65, max-width 68ch
  - Small / Metadata: 0.75rem (12px) – 0.8125rem (13px), line-height 1.5

## Layout & Rhythm

- **Max Measure:** Main column 48rem (768px) to 56rem (896px) for optimal reading cadence.
- **Vertical Spacing:** Generous separation between sections (4rem to 5.5rem). More space above headings than below them.
- **Borders:** Thin 1px solid `#DDD8CE`, subtle and functional without heavy shadows.
- **Cards & Enclosures:** Used sparingly; prefer whitespace, rule lines, and baseline alignments over heavy boxes.

## Component Conventions

- **Links:** `#8C3A27` with underline offset 3px, or `#1C1B18` with subtle transition.
- **Flow Diagrams:** Horizontal flex sequence with official SVG brand marks, muted connector arrows, and a highlighted human review checkpoint.
- **Screenshot Viewer:** Clean lightboxed or tabbed view showing real app captures with descriptive captions.
- **Video Player:** Native HTML5 `<video>` with custom poster frame and quiet play controls.
