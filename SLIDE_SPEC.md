# Banking for Block — 72nd Board of Directors Meeting
## Slide Specification Document

> **Purpose:** This document is a pixel-level specification for a 3-slide board presentation on Banking. A designer should be able to build production-ready Figma frames from this document alone, without follow-up questions.

---

## Table of Contents

1. [Global Specifications](#global-specifications)
2. [Slide 1 — Banking is working — and Q1 proves it](#slide-1)
3. [Slide 2 — We're turning Square into the only financial account sellers need](#slide-2)
4. [Slide 3 — Cash App is becoming the account people live in](#slide-3)
5. [Asset Pull List (Master)](#asset-pull-list-master)
6. [Appendix: Color Tokens & Typography Scale](#appendix)

---

<a id="global-specifications"></a>
## Global Specifications

### Canvas

| Property | Value |
|---|---|
| Aspect ratio | 16:9 |
| Resolution | 1920 × 1080 px |
| Safe margin (all sides) | 80 px (top/bottom), 96 px (left/right) |
| Usable content area | 1728 × 920 px |
| Grid | 12-column, 24 px gutter, aligned to safe margin |
| Baseline grid | 8 px increments for all spacing |

### Brand Color Tokens

| Token Name | Hex | Usage |
|---|---|---|
| `block-black` | `#000000` | Primary text, slide backgrounds (dark variant) |
| `block-white` | `#FFFFFF` | Light backgrounds, reversed text on dark |
| `square-blue` | `#006AFF` | Square-specific metrics, chart lines, accents |
| `cash-green` | `#00D632` | Cash App-specific metrics, chart lines, accents |
| `gray-900` | `#1A1A1A` | Secondary text on light backgrounds |
| `gray-700` | `#4A4A4A` | Body copy on light backgrounds |
| `gray-400` | `#999999` | Tertiary text, axis labels, captions |
| `gray-200` | `#E5E5E5` | Divider lines, card borders |
| `gray-100` | `#F5F5F5` | Card/panel fill on white backgrounds |
| `beat-green` | `#00C853` | "Above plan" / positive delta callouts |
| `miss-red` | `#FF3B30` | "Below plan" callouts (not used in this deck) |
| `highlight-yellow` | `#FFD60A` | Spotlight/pulse annotation on charts |

### Typography Scale

All type is set in **Inter** (primary) or **SF Pro Display** (fallback). No other typefaces.

| Role | Font | Weight | Size | Line Height | Letter Spacing | Color |
|---|---|---|---|---|---|---|
| Slide headline (H1) | Inter | Bold (700) | 48 px | 56 px (1.17×) | −0.02 em | `block-black` |
| Slide subheadline (H2) | Inter | Medium (500) | 26 px | 34 px (1.31×) | 0 em | `gray-700` |
| Section label (H3) | Inter | SemiBold (600) | 20 px | 28 px (1.4×) | 0.04 em (uppercase) | `gray-400` or brand color |
| Body copy | Inter | Regular (400) | 17 px | 26 px (1.53×) | 0 em | `gray-700` |
| Metric number (hero) | Inter | Bold (700) | 68 px | 72 px (1.06×) | −0.03 em | `block-black` |
| Metric number (secondary) | Inter | Bold (700) | 40 px | 48 px (1.2×) | −0.02 em | `block-black` |
| Metric label | Inter | Medium (500) | 14 px | 20 px (1.43×) | 0.06 em (uppercase) | `gray-400` |
| Metric delta (badge) | Inter | SemiBold (600) | 14 px | 20 px | 0 em | `beat-green` or `block-white` on green pill |
| Chart axis label | Inter | Regular (400) | 12 px | 16 px | 0.02 em | `gray-400` |
| Chart data label | Inter | SemiBold (600) | 13 px | 16 px | 0 em | `block-black` |
| Transition text / footer | Inter | Regular (400) | 15 px | 22 px | 0 em | `gray-400` |
| Slide number | Inter | Medium (500) | 12 px | 16 px | 0.04 em | `gray-400` |

### Shared Layout Rules

- **Slide number** is always bottom-right, 96 px from right edge, 40 px from bottom edge.
- **Block logo** (wordmark, black) is always top-left, 96 px from left, 48 px from top, 80 px wide.
- **Headline** starts at y = 136 px (below logo + 8 px spacing), left-aligned to column 1.
- **Subheadline** starts 12 px below headline baseline.
- **Content area** begins at y = 260 px (below subheadline + 40 px breathing room).
- **Transition text** (when present) is pinned 48 px above bottom safe margin, full width, center-aligned.
- All cards/panels use 16 px border-radius, 1 px `gray-200` stroke OR `gray-100` fill (no stroke). Never both.

### Chart Conventions

- Line charts: 2.5 px stroke, rounded caps, rounded joins.
- Data points on lines: 6 px diameter circles, filled with line color, 2 px white stroke.
- Highlighted data point (e.g., Q1 beat): 10 px diameter, pulsing ring annotation in `highlight-yellow` at 40% opacity, 20 px outer ring.
- Bar charts: 8 px border-radius top corners, 32 px default bar width.
- Grid lines: 1 px `gray-200`, dashed (4 px dash, 4 px gap). No vertical grid lines.
- Y-axis on left, X-axis on bottom. No chart borders/outlines.
- Legend: horizontal, top-right of chart area, using 8 px colored circles + label.

### Animation / Build Notes (for Keynote/GSlides export)

- Each slide builds in 2–3 steps (noted per slide below).
- Default transition between slides: **Fade**, 0.4 s, ease-in-out.
- Within-slide builds: **Appear** (no motion), 0.3 s, triggered on click.

---

<a id="slide-1"></a>
## Slide 1 — "Banking is working — and Q1 proves it"

### 1.1 Purpose & Narrative

This is the **opening frame**. It establishes that Banking — across both Square and Cash App — is delivering. The audience should leave this slide with one takeaway: *"$1B+ in combined Banking GP, both sides beating plan."* The tone is confident, data-forward, and brief. No deep product detail — that comes in Slides 2 and 3.

---

### 1.2 Exact Copy

#### Headline (H1)
```
$1B+ in combined Banking GP. Both sides beating plan.
```

#### Subheadline (H2)
```
Banking is Block's bet that we can become the primary financial relationship for both sellers and consumers. Q1 is the strongest evidence yet.
```

#### Scorecard Metrics (left panel, top to bottom)

Each metric is displayed as a **metric card** with three text elements: **number**, **label**, and **delta badge**.

| # | Metric Number | Metric Label | Delta Badge |
|---|---|---|---|
| 1 | `~$98M` | SQUARE BANKING GP | `+21% YoY · +5% above AP` |
| 2 | `$913M` | CASH APP BANKING GP | `+9% YoY` |
| 3 | `$15.5B` | CARD GPV (MARCH) — ALL-TIME HIGH | `+21% YoY` |
| 4 | `9.7M` | PRIMARY BANKING ACTIVES — HIGHEST MONTH EVER | `↑ record` |
| 5 | `861K` | NEW CARD ACTIVES (MARCH) | `+17% YoY` |

> **Copy note:** "AP" = Annual Plan. The board is familiar with this abbreviation. "All-time high" and "highest month ever" are appended to the label in a lighter weight to serve as contextual qualifiers.

#### Transition Text (bottom)
```
Growth is strong, but we're still early in capturing the full financial life of our customers.
```

---

### 1.3 Layout Grid Description

```
┌──────────────────────────────────────────────────────────────────┐
│  [Block logo]                                         [Slide 1] │
│                                                                  │
│  HEADLINE (H1) — spans columns 1–12 (full width)                │
│  SUBHEADLINE (H2) — spans columns 1–8 (66% width)               │
│                                                                  │
│  ┌─────────────────────────┐  ┌────────────────────────────────┐ │
│  │                         │  │                                │ │
│  │   SCORECARD PANEL       │  │   CHART PANEL                  │ │
│  │   (Columns 1–5)         │  │   (Columns 6–12)               │ │
│  │   40% width             │  │   60% width                    │ │
│  │                         │  │                                │ │
│  │   5 metric cards        │  │   Combined Banking GP          │ │
│  │   stacked vertically    │  │   trendline chart              │ │
│  │   16px gap between      │  │                                │ │
│  │                         │  │                                │ │
│  └─────────────────────────┘  └────────────────────────────────┘ │
│                                                                  │
│         "Growth is strong, but we're still early …"              │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

#### Precise Measurements

| Element | X | Y | Width | Height | Notes |
|---|---|---|---|---|---|
| Block logo | 96 px | 48 px | 80 px | auto | SVG wordmark, black |
| Slide number "1" | 1792 px | 1008 px | auto | auto | Right-aligned |
| Headline | 96 px | 136 px | 1728 px | auto | Left-aligned, single line preferred; wrap OK |
| Subheadline | 96 px | 200 px | 1152 px (cols 1–8) | auto | Max 2 lines |
| Scorecard panel | 96 px | 280 px | 672 px (cols 1–5) | 600 px | Contains 5 metric cards |
| Chart panel | 816 px | 280 px | 912 px (cols 6–12) | 600 px | Contains trendline chart |
| Transition text | 96 px | 940 px | 1728 px | auto | Center-aligned |

#### Scorecard Card Spec (each card)

| Property | Value |
|---|---|
| Card width | 672 px (full panel width) |
| Card height | 104 px |
| Card fill | `gray-100` (`#F5F5F5`) |
| Card corner radius | 16 px |
| Card internal padding | 24 px left/right, 16 px top/bottom |
| Gap between cards | 16 px |
| Metric number | Left-aligned, vertically centered, `metric-number-secondary` style (40 px bold) |
| Metric label | Right of number, baseline-aligned, `metric-label` style (14 px uppercase) |
| Delta badge | Far right, vertically centered, pill shape: 24 px height, 12 px horizontal padding, 999 px border-radius, `beat-green` fill, white text `metric-delta` style |

> **Special treatment for cards 3 and 4:** Append the qualifier text ("ALL-TIME HIGH" / "HIGHEST MONTH EVER") after the label with an em-dash separator. Use `beat-green` color for the qualifier portion only.

---

### 1.4 Chart Specification — Combined Banking GP Trendline

| Property | Value |
|---|---|
| Chart type | Dual-line chart (two series) with shared X-axis |
| Chart area | 912 × 480 px (within chart panel, 24 px internal padding) |
| Series 1 | **Square Banking GP** — `square-blue` (`#006AFF`), 2.5 px stroke |
| Series 2 | **Cash App Banking GP** — `cash-green` (`#00D632`), 2.5 px stroke |
| X-axis | Quarters: `Q4 '24`, `Q1 '25`, `Q2 '25`, `Q3 '25`, `Q4 '25`, `Q1 '26` (6 data points) |
| Y-axis | Dollar values in $M. Range: $0 – $1,100M. Gridlines at $200M increments. |
| Data points (approximate — source from finance) | See table below |
| Q1 '26 highlight | Both Q1 '26 data points get the **pulsing ring annotation** (`highlight-yellow`). Draw a light vertical dashed line at Q1 '26 in `highlight-yellow` at 30% opacity spanning full chart height. |
| Annotation callout | Above the Q1 '26 data cluster, place a callout box: white fill, 1 px `gray-200` border, 12 px padding, 12 px border-radius. Text inside: `"Q1 '26: $1.01B combined"` in `chart-data-label` style. Arrow pointing down to the data points. |
| Legend | Top-right of chart area. Two items: blue circle + "Square Banking GP", green circle + "Cash App Banking GP". |
| Background | `block-white`, no chart border |

#### Approximate Data Points (validate with Finance before final build)

| Quarter | Square Banking GP ($M) | Cash App Banking GP ($M) |
|---|---|---|
| Q4 '24 | ~78 | ~830 |
| Q1 '25 | ~81 | ~838 |
| Q2 '25 | ~85 | ~855 |
| Q3 '25 | ~89 | ~875 |
| Q4 '25 | ~93 | ~895 |
| Q1 '26 | ~98 | ~913 |

> **Note:** These are illustrative trend values. The designer should leave the data layer editable so Finance can drop in actuals. The visual shape (steady upward trend, Q1 '26 as highest) is what matters for layout purposes.

---

### 1.5 Color Usage Notes

- **Background:** `block-white` (`#FFFFFF`).
- **All text** defaults to `block-black` or `gray-700` per the typography table.
- **Scorecard cards** use `gray-100` fill — no strokes.
- **Delta badges** use `beat-green` fill with `block-white` text.
- **Chart lines** are the only places `square-blue` and `cash-green` appear on this slide.
- **No gradients** anywhere on this slide.

---

### 1.6 Build / Animation Sequence

| Step | What Appears | Timing |
|---|---|---|
| Build 0 (on slide enter) | Logo, slide number, headline, subheadline | Immediate |
| Build 1 (click) | All 5 scorecard cards fade in simultaneously | 0.3 s appear |
| Build 2 (click) | Chart draws in (line animation left→right, 0.8 s ease-out), then Q1 annotation pops | 0.8 s + 0.3 s |
| Build 3 (click) | Transition text fades in at bottom | 0.3 s appear |

---

<a id="slide-2"></a>
## Slide 2 — "We're turning Square into the only financial account sellers need"

### 2.1 Purpose & Narrative

This slide tells the **Square Banking flywheel story**. The audience should understand that Square Banking is not a collection of disconnected products — it's a closed-loop financial system where each product feeds the next. The three "acts" map to acquisition → spend → deposits, forming a self-reinforcing cycle.

---

### 2.2 Exact Copy

#### Headline (H1)
```
We're turning Square into the only financial account sellers need
```

#### Subheadline (H2)
```
Most Square sellers still split their financial life across multiple banks, credit cards, and bill pay tools. Every dollar that leaves our ecosystem is a dollar we don't monetize. In Q1 we pulled dollars back in. In Q2, we close the loop.
```

#### Act 1 — Section Label (H3)
```
ACT 1 — GET SELLERS IN THE DOOR (Q1)
```
Color: `square-blue`

#### Act 1 — Body Bullets
```
• ChAD now reaches 61% of new payments customers (up from 42% in Dec)
• Sellers who see ChAD are 52% more likely to activate checking in month 1
• Zero drag on payment sign-up rates
```

#### Act 2 — Section Label (H3)
```
ACT 2 — MAKE EVERY DOLLAR FLOW THROUGH SQUARE (Q1→Q2)
```
Color: `square-blue`

#### Act 2 — Body Bullets
```
• Square Credit Card: >50K active cards, ~$300M extended credit
• 1.5% cash back (7–10% conversion lift in testing)
• Q2: 100% of eligible sellers, targeting $1B annualized spend
• Pay Anyone: sellers pay ANY vendor via Credit Card — Square delivers via ACH/check
• Turns Credit Card into a full AP solution — every outflow monetizable
```

#### Act 3 — Section Label (H3)
```
ACT 3 — FUND IT ALL WITH DEPOSITS (Q2)
```
Color: `square-blue`

#### Act 3 — Body Bullets
```
• High Yield Savings launches mid-May, 3.5–3.75% APY
• Target: >$1B in core deposits
• Deposits fund lending → better credit terms → more card usage → Pay Anyone expands spend
```

#### Demo Callout (small, bottom-left)
```
▶ DEMO: Pay Anyone flow walkthrough
```

---

### 2.3 Layout Grid Description

This slide uses a **left-text / right-visual split**, with the text column scrolling through three acts and the right column holding the flywheel diagram (primary) with a smaller credit card chart below it.

```
┌──────────────────────────────────────────────────────────────────┐
│  [Block logo]                                         [Slide 2] │
│                                                                  │
│  HEADLINE (H1) — spans columns 1–12 (full width)                │
│  SUBHEADLINE (H2) — spans columns 1–7 (58% width)               │
│                                                                  │
│  ┌──────────────────────┐  ┌──────────────────────────────────┐  │
│  │                      │  │                                  │  │
│  │  TEXT COLUMN          │  │  VISUAL COLUMN                  │  │
│  │  (Columns 1–5)       │  │  (Columns 6–12)                 │  │
│  │  40% width           │  │  60% width                      │  │
│  │                      │  │                                  │  │
│  │  ACT 1 section       │  │  ┌──────────────────────────┐   │  │
│  │  ── thin divider ──  │  │  │  FLYWHEEL DIAGRAM        │   │  │
│  │  ACT 2 section       │  │  │  (Primary Visual)        │   │  │
│  │  ── thin divider ──  │  │  │  480 × 400 px            │   │  │
│  │  ACT 3 section       │  │  └──────────────────────────┘   │  │
│  │                      │  │  ┌──────────────────────────┐   │  │
│  │                      │  │  │  CREDIT CARD GROWTH      │   │  │
│  │                      │  │  │  (Secondary Chart)       │   │  │
│  │                      │  │  │  480 × 180 px            │   │  │
│  └──────────────────────┘  │  └──────────────────────────┘   │  │
│                            └──────────────────────────────────┘  │
│  ▶ DEMO: Pay Anyone flow walkthrough                             │
└──────────────────────────────────────────────────────────────────┘
```

#### Precise Measurements

| Element | X | Y | Width | Height | Notes |
|---|---|---|---|---|---|
| Headline | 96 px | 136 px | 1728 px | auto | May wrap to 2 lines — OK |
| Subheadline | 96 px | 208 px | 1008 px (cols 1–7) | auto | Max 3 lines |
| Text column | 96 px | 296 px | 672 px | 600 px | Vertically, 3 acts stacked |
| Act 1 block | 96 px | 296 px | 672 px | ~160 px | Label + 3 bullets |
| Divider 1 | 96 px | 464 px | 672 px | 1 px | `gray-200` |
| Act 2 block | 96 px | 480 px | 672 px | ~200 px | Label + 5 bullets |
| Divider 2 | 96 px | 688 px | 672 px | 1 px | `gray-200` |
| Act 3 block | 96 px | 704 px | 672 px | ~140 px | Label + 3 bullets |
| Visual column | 816 px | 296 px | 912 px | 600 px | Contains flywheel + chart |
| Flywheel diagram | 816 px | 296 px | 912 px | 400 px | See spec below |
| Credit card chart | 816 px | 720 px | 912 px | 180 px | See spec below |
| Demo callout | 96 px | 940 px | auto | auto | Left-aligned |

#### Act Section Internal Spec

| Element | Spec |
|---|---|
| Section label (H3) | `square-blue`, uppercase, 20 px SemiBold, 0.04 em tracking |
| Gap: label → first bullet | 12 px |
| Bullet style | 6 px filled circle, `square-blue`, aligned to first line baseline, 16 px indent |
| Bullet text | `body` style (17 px Regular, `gray-700`) |
| Gap between bullets | 8 px |

---

### 2.4 Primary Visual — Flywheel Diagram

#### Diagram Description

A **circular flywheel** with 5 nodes connected by curved directional arrows forming a clockwise loop. The flywheel sits centered within its 912 × 400 px container.

| Property | Value |
|---|---|
| Flywheel diameter | 320 px (outer edge of node positions) |
| Center point | 456 px from left edge of container, 200 px from top |
| Arrow style | 3 px stroke, `square-blue` at 60% opacity, rounded, with arrowhead (8 px equilateral triangle) |
| Arrow path | Curved (arc between nodes), clockwise direction |
| Node style | Rounded rectangle, 160 × 56 px, 12 px border-radius, `square-blue` fill, white text |
| Node text style | Inter SemiBold 14 px, `block-white`, centered |

#### Node Positions & Labels (clockwise from top)

| # | Label (Line 1) | Label (Line 2 — smaller) | Clock Position |
|---|---|---|---|
| 1 | `ChAD` | `Acquisition` | 12 o'clock (top center) |
| 2 | `Credit Card` | `Spend` | 2 o'clock (top-right) |
| 3 | `Pay Anyone` | `All Outflows` | 5 o'clock (bottom-right) |
| 4 | `High Yield Savings` | `Deposits` | 7 o'clock (bottom-left) |
| 5 | `Lending` | `Back to Credit Card` | 10 o'clock (top-left) |

> Line 2 in each node is Inter Regular 11 px, `block-white` at 80% opacity, 4 px below Line 1.

#### Flywheel Center

Place a subtle text label in the center of the flywheel ring:

```
THE SQUARE
BANKING LOOP
```
Inter Medium 13 px, `gray-400`, center-aligned, 2 lines.

#### Flywheel Build Animation

The flywheel builds node-by-node clockwise (ChAD → Credit Card → Pay Anyone → HYS → Lending), each node appearing with its incoming arrow. 0.2 s per node, 0.1 s gap = ~1.5 s total.

---

### 2.5 Secondary Visual — Credit Card Growth Trajectory

| Property | Value |
|---|---|
| Chart type | Area chart (single series) with target line |
| Chart area | 864 × 140 px (within 912 × 180 container, 24 px padding) |
| Series | **Annualized Credit Card Spend** — `square-blue` fill at 15% opacity, `square-blue` 2 px stroke |
| X-axis | Months: `Jan '26`, `Feb`, `Mar`, `Apr`, `May`, `Jun` (Q1 actual + Q2 projected) |
| Y-axis | $0 – $1.2B. Gridlines at $250M increments. |
| Data shape | Upward curve from ~$600M annualized (Jan) → ~$750M (Mar) → projected ~$1B (Jun) |
| Q2 projection | Dashed line from Mar→Jun, `square-blue` at 50% opacity |
| Target line | Horizontal dashed line at $1B, `highlight-yellow`, label: `"$1B target"` right-aligned |
| Chart title | `"Credit Card — Annualized Spend Trajectory"` in `section-label` style, above chart, left-aligned |

---

### 2.6 Color Usage Notes

- **Background:** `block-white` (`#FFFFFF`).
- **`square-blue`** is the dominant accent color on this slide — section labels, bullet dots, flywheel nodes, chart line.
- **No `cash-green`** appears on this slide (this is the Square story).
- Flywheel arrows use `square-blue` at 60% to avoid visual heaviness.
- The area chart fill is `square-blue` at 15% — subtle, not overwhelming.
- Dividers between acts are `gray-200` (1 px).

---

### 2.7 Asset Pull List

| Asset | Source | Notes |
|---|---|---|
| Pay Anyone demo recording | Product team / internal demo repo | 30–60 second screen recording of the Pay Anyone flow. Needed for live demo or embedded video fallback. |
| Square Credit Card product shot | Brand asset library | Physical card render, angled, on white. Used as optional inset in flywheel "Credit Card" node. |
| ChAD screenshot | Growth team | Screenshot of the ChAD prompt as it appears during payments onboarding. Optional: small inset near Act 1. |
| High Yield Savings UI mock | Square Banking PM | Pre-launch mock of the HYS dashboard. Optional: small inset near Act 3. |

---

### 2.8 Build / Animation Sequence

| Step | What Appears | Timing |
|---|---|---|
| Build 0 (on slide enter) | Logo, slide number, headline, subheadline | Immediate |
| Build 1 (click) | Act 1 section (label + bullets) + flywheel node 1 (ChAD) | 0.3 s |
| Build 2 (click) | Act 2 section + flywheel nodes 2–3 (Credit Card, Pay Anyone) + Credit Card chart | 0.5 s |
| Build 3 (click) | Act 3 section + flywheel nodes 4–5 (HYS, Lending) + loop closes | 0.5 s |
| Build 4 (click) | Demo callout appears at bottom | 0.3 s |

---

<a id="slide-3"></a>
## Slide 3 — "Cash App is becoming the account people live in"

### 3.1 Purpose & Narrative

This slide makes the case that Cash App Banking is evolving from a card product into a **full financial account** with compounding stickiness. The "layers" metaphor is deliberate: each layer makes the account harder to leave. The audience should feel that Cash App is building structural moats, not just features.

---

### 3.2 Exact Copy

#### Headline (H1)
```
Cash App is becoming the account people live in
```

#### Subheadline (H2)
```
Cash App Banking's growth has been driven by the Card. But a card alone isn't a bank. The story is about turning Cash App into something competitors can't replicate: an account so embedded in daily life that switching costs become real.
```

#### Layer 1 — Section Label (H3)
```
LAYER 1 — THE CARD GETS SMARTER (Q1)
```
Color: `cash-green`

#### Layer 1 — Body Bullets
```
• Debit Flex: ~50K customers, single card flexes debit ↔ credit
• Digital wallet provisioning: up 8 pts to 62.3%
• Digital wallet GPV: 19% → 24% of total card GPV
```

#### Layer 2 — Section Label (H3)
```
LAYER 2 — MONEY MOVES MORE EASILY (Q1)
```
Color: `cash-green`

#### Layer 2 — Body Bullets
```
• Transfers: Apple Pay, Google Pay, ACH for BTC, multi-card
• Instant Transfer fee update: +$18M above plan
• Apex migration: >10M accounts to scalable clearing
```

#### Layer 3 — Section Label (H3)
```
LAYER 3 — ESSENTIAL INFRASTRUCTURE (Q2)
```
Color: `cash-green`

#### Layer 3 — Body Bullets
```
• Cash App Tags: First NFC payment device, May 21 launch, ~20K units
• Phone Plans: AT&T $40/month, ~$250M GP over 3 years
• Green Evolution: Membership wrapper, solving 37% retention gap
```

#### Demo Callout (small, bottom-left)
```
▶ DEMO: Cash App Tag tapping at terminal
```

---

### 3.3 Layout Grid Description

Same **left-text / right-visual split** as Slide 2 for deck consistency, but the right column holds the stacking layer diagram (primary) and the Primary Banking Actives trajectory (secondary).

```
┌──────────────────────────────────────────────────────────────────┐
│  [Block logo]                                         [Slide 3] │
│                                                                  │
│  HEADLINE (H1) — spans columns 1–12 (full width)                │
│  SUBHEADLINE (H2) — spans columns 1–7 (58% width)               │
│                                                                  │
│  ┌──────────────────────┐  ┌──────────────────────────────────┐  │
│  │                      │  │                                  │  │
│  │  TEXT COLUMN          │  │  VISUAL COLUMN                  │  │
│  │  (Columns 1–5)       │  │  (Columns 6–12)                 │  │
│  │  40% width           │  │  60% width                      │  │
│  │                      │  │                                  │  │
│  │  LAYER 1 section     │  │  ┌──────────────────────────┐   │  │
│  │  ── thin divider ──  │  │  │  STACKING LAYER DIAGRAM  │   │  │
│  │  LAYER 2 section     │  │  │  (Primary Visual)        │   │  │
│  │  ── thin divider ──  │  │  │  480 × 400 px            │   │  │
│  │  LAYER 3 section     │  │  └──────────────────────────┘   │  │
│  │                      │  │  ┌──────────────────────────┐   │  │
│  │                      │  │  │  PRIMARY BANKING ACTIVES │   │  │
│  │                      │  │  │  (Secondary Chart)       │   │  │
│  │                      │  │  │  480 × 180 px            │   │  │
│  └──────────────────────┘  │  └──────────────────────────┘   │  │
│                            └──────────────────────────────────┘  │
│  ▶ DEMO: Cash App Tag tapping at terminal                        │
└──────────────────────────────────────────────────────────────────┘
```

#### Precise Measurements

| Element | X | Y | Width | Height | Notes |
|---|---|---|---|---|---|
| Headline | 96 px | 136 px | 1728 px | auto | May wrap to 2 lines |
| Subheadline | 96 px | 208 px | 1008 px | auto | Max 3 lines |
| Text column | 96 px | 312 px | 672 px | 580 px | 3 layers stacked |
| Layer 1 block | 96 px | 312 px | 672 px | ~140 px | Label + 3 bullets |
| Divider 1 | 96 px | 460 px | 672 px | 1 px | `gray-200` |
| Layer 2 block | 96 px | 476 px | 672 px | ~140 px | Label + 3 bullets |
| Divider 2 | 96 px | 624 px | 672 px | 1 px | `gray-200` |
| Layer 3 block | 96 px | 640 px | 672 px | ~140 px | Label + 3 bullets |
| Visual column | 816 px | 312 px | 912 px | 580 px | Contains layer diagram + chart |
| Stacking diagram | 816 px | 312 px | 912 px | 380 px | See spec below |
| Actives chart | 816 px | 716 px | 912 px | 180 px | See spec below |
| Demo callout | 96 px | 940 px | auto | auto | Left-aligned |

#### Layer Section Internal Spec

Identical structure to Slide 2's Act sections, but with `cash-green` replacing `square-blue` for section labels and bullet dots.

---

### 3.4 Primary Visual — Stacking Layer Diagram

#### Diagram Description

A **vertical stack of 6 horizontal bars**, building from bottom to top like geological strata. Each bar represents a product/feature layer. The bottom bar is the widest and most saturated; layers get progressively lighter in fill as they go up, creating a "building" visual metaphor. The topmost layer (Green) acts as a wrapper that encompasses all others.

| Property | Value |
|---|---|
| Container | 912 × 380 px |
| Bar width | 720 px (centered in container, 96 px margin each side) |
| Bar height | 48 px each |
| Bar gap | 8 px |
| Bar corner radius | 12 px |
| Total stack height | (6 × 48) + (5 × 8) = 328 px |
| Stack vertical position | Centered in container (26 px top/bottom padding) |

#### Layer Bars (bottom to top)

| # | Label | Fill Color | Text Color | Opacity | Position |
|---|---|---|---|---|---|
| 1 (bottom) | `Cash App Card` | `cash-green` | `block-white` | 100% | Base |
| 2 | `Digital Wallets` | `cash-green` | `block-white` | 85% | +56 px |
| 3 | `Debit Flex` | `cash-green` | `block-white` | 70% | +112 px |
| 4 | `Cash App Tags` | `cash-green` | `block-white` | 55% | +168 px |
| 5 | `Phone Plans` | `cash-green` | `block-white` | 40% | +224 px |
| 6 (top) | `Green (Membership Wrapper)` | `cash-green` | `block-white` | 100%, 2 px dashed border | +280 px |

> **Layer 6 special treatment:** The "Green" bar is rendered as a **dashed outline** (2 px `cash-green` dashed stroke, 4 px dash/4 px gap) with `cash-green` at 10% fill, to indicate it's the upcoming wrapper that will enclose everything. This visually distinguishes it as "in progress."

#### Bar Label Spec

- Text: Inter SemiBold 15 px, centered vertically and horizontally within bar.
- For Layer 6, append a small badge: `"Q2"` in a 20 × 16 px pill, `cash-green` fill at 30%, Inter Medium 10 px, 8 px to the right of the label text.

#### Annotation Arrows

Draw thin annotation lines (1 px `gray-400`) from the left edge of each bar to the corresponding Layer section in the text column. These are subtle visual connectors:
- Horizontal line from bar left edge → extends left → turns down/up to align with the Layer label's Y position.
- Use 90° elbow joints, not diagonal lines.
- These connectors are optional — include only if they don't create visual clutter. Designer's discretion.

---

### 3.5 Secondary Visual — Primary Banking Actives Trajectory

| Property | Value |
|---|---|
| Chart type | Line chart (single series) with goal line |
| Chart area | 864 × 140 px (within 912 × 180 container, 24 px padding) |
| Series | **Primary Banking Actives** — `cash-green`, 2.5 px stroke, filled area at 12% opacity |
| X-axis | Months: `Oct '25`, `Nov`, `Dec`, `Jan '26`, `Feb`, `Mar`, `Apr*`, `May*`, `Jun*` |
| Y-axis | 0 – 11M. Gridlines at 2M increments. |
| Data shape | Upward trend from ~8.5M (Oct) → 9.7M (Mar) → projected ~10M+ (Jun) |
| Projection | Dashed line from Mar→Jun, `cash-green` at 50% opacity |
| Goal line | Horizontal dashed line at 10M, `highlight-yellow`, label: `"10M goal"` right-aligned |
| March callout | Small annotation at March data point: `"9.7M — record"` in `chart-data-label` style, with `beat-green` dot |
| Chart title | `"Primary Banking Actives — Path to 10M"` in `section-label` style, above chart, left-aligned |
| Asterisk note | Below chart, right-aligned, 11 px Inter Regular `gray-400`: `"* Projected"` |

---

### 3.6 Color Usage Notes

- **Background:** `block-white` (`#FFFFFF`).
- **`cash-green`** is the dominant accent color — section labels, bullet dots, stacking bars, chart line.
- **No `square-blue`** appears on this slide (this is the Cash App story).
- The stacking bars use decreasing opacity to create depth without introducing new colors.
- The Green (Layer 6) dashed border treatment is the only place a dashed stroke appears in the diagram.
- Goal line uses `highlight-yellow` for consistency with Slide 1's annotation treatment.

---

### 3.7 Asset Pull List

| Asset | Source | Notes |
|---|---|---|
| Cash App Tag product photo | Hardware team / Brand asset library | High-res photo of the physical NFC tag. Ideally lifestyle shot of tag tapping at a terminal. Could be used as a small inset (120 × 120 px) near Layer 3, or as the demo still. |
| Cash App Tag demo video | Product marketing | 15–30 second clip of tag tapping at a Square Terminal. For live demo or embedded video fallback. |
| Cash App Card render | Brand asset library | Physical card render, angled, on white. Used as optional inset in the base layer of the stacking diagram. |
| Green membership UI mock | Cash App PM | Pre-launch mock of the Green membership wrapper. Optional: small inset near Layer 3. |
| Phone Plans partnership lockup | BD team | AT&T + Cash App co-branded lockup if available. Optional. |

---

### 3.8 Build / Animation Sequence

| Step | What Appears | Timing |
|---|---|---|
| Build 0 (on slide enter) | Logo, slide number, headline, subheadline | Immediate |
| Build 1 (click) | Layer 1 text + stacking bar 1 (Card) slides up from bottom | 0.3 s |
| Build 2 (click) | Layer 2 text + stacking bars 2–3 (Wallets, Debit Flex) stack on | 0.4 s |
| Build 3 (click) | Layer 3 text + stacking bars 4–6 (Tags, Phone Plans, Green wrapper) + Actives chart draws in | 0.6 s |
| Build 4 (click) | Demo callout appears at bottom | 0.3 s |

---

<a id="asset-pull-list-master"></a>
## Asset Pull List (Master)

Consolidated list of all assets needed across all 3 slides. Assign an owner and due date for each.

| # | Asset | Slide(s) | Source / Owner | Format | Status |
|---|---|---|---|---|---|
| 1 | Block wordmark (black, SVG) | 1, 2, 3 | Brand team | SVG | ☐ |
| 2 | Combined Banking GP quarterly data (actuals) | 1 | Finance | CSV/Sheet | ☐ |
| 3 | Pay Anyone demo recording | 2 | Square Banking PM | MP4, 1080p | ☐ |
| 4 | Square Credit Card product render | 2 | Brand asset library | PNG, 2x | ☐ |
| 5 | ChAD onboarding screenshot | 2 | Growth team | PNG, 2x | ☐ |
| 6 | High Yield Savings UI mock | 2 | Square Banking PM | PNG/Figma | ☐ |
| 7 | Credit Card annualized spend data | 2 | Finance | CSV/Sheet | ☐ |
| 8 | Cash App Tag product photo | 3 | Hardware team | PNG, 2x | ☐ |
| 9 | Cash App Tag demo video | 3 | Product marketing | MP4, 1080p | ☐ |
| 10 | Cash App Card render | 3 | Brand asset library | PNG, 2x | ☐ |
| 11 | Green membership UI mock | 3 | Cash App PM | PNG/Figma | ☐ |
| 12 | Phone Plans AT&T lockup | 3 | BD team | SVG/PNG | ☐ |
| 13 | Primary Banking Actives monthly data | 3 | Finance | CSV/Sheet | ☐ |

---

<a id="appendix"></a>
## Appendix: Color Tokens & Typography Scale (Quick Reference)

### Color Palette (Visual Swatch Guide)

```
██████  #000000  block-black       Primary text, dark backgrounds
██████  #FFFFFF  block-white       Light backgrounds, reversed text
██████  #006AFF  square-blue       Square metrics, accents
██████  #00D632  cash-green        Cash App metrics, accents
██████  #1A1A1A  gray-900          Secondary text
██████  #4A4A4A  gray-700          Body copy
██████  #999999  gray-400          Tertiary text, captions
██████  #E5E5E5  gray-200          Dividers, borders
██████  #F5F5F5  gray-100          Card/panel fills
██████  #00C853  beat-green        Positive deltas
██████  #FF3B30  miss-red          Negative deltas (unused)
██████  #FFD60A  highlight-yellow  Annotations, targets
```

### Type Scale (Visual Hierarchy)

```
68px  Bold   ← Hero metric numbers ($913M, 9.7M)
48px  Bold   ← Slide headlines
40px  Bold   ← Secondary metric numbers (~$98M)
26px  Medium ← Subheadlines
20px  Semi   ← Section labels (ACT 1, LAYER 1)
17px  Regular← Body copy / bullets
15px  Regular← Transition text / footer
14px  Semi   ← Delta badges, metric labels
13px  Semi   ← Chart data labels
12px  Regular← Chart axis labels, slide numbers
11px  Regular← Fine print / asterisk notes
```

---

## Revision History

| Date | Author | Change |
|---|---|---|
| 2026-04-21 | — | Initial spec created |

---

*End of specification document.*


---

<a id="product-mockups"></a>
## Product Experience Mockups — Asset Placement Guide

> **Purpose:** Each slide now includes high-fidelity CSS mockups as placeholders. This section specifies exactly what real assets should replace them, where to source them, and the exact dimensions/framing needed.

---

### Slide 2 — Square Banking Product Experiences

#### Mockup Position 1: ChAD Onboarding (Bottom-left, under Act 1 column)

| Property | Specification |
|---|---|
| **Frame type** | Browser/laptop frame |
| **Dimensions** | ~480 × 300 px content area |
| **What to replace with** | Screenshot of the Square Dashboard ChAD onboarding modal as seen by a Sole Proprietor on web |
| **Source owner** | Square Banking — ChAD team |
| **Framing notes** | Capture the modal/card overlay on the Dashboard. Include the "Set up Square Checking" headline and CTA button. Crop to just the modal + slight Dashboard background blur. |
| **Fallback** | If screenshot unavailable, use the CSS mockup as-is — it's representative enough for board context |

#### Mockup Position 2: Pay Anyone Flow (Bottom-center, under Act 2 column — HERO POSITION)

| Property | Specification |
|---|---|
| **Frame type** | Browser/laptop frame (larger than others) |
| **Dimensions** | ~540 × 340 px content area |
| **What to replace with** | Screenshot or screen recording still of the Pay Anyone bill payment flow showing: vendor search → payment via Square Credit Card → ACH delivery confirmation |
| **Source owner** | Square Banking — Bill Pay / Pay Anyone team |
| **Framing notes** | Ideal: 2-3 step flow shown side by side (search → confirm → success). If single screenshot, capture the payment confirmation screen showing the Credit Card as payment method, vendor name, amount, delivery method, and cash back earned. |
| **Why this is hero** | This is the single most important product moment in the deck. It demonstrates the Credit Card + Pay Anyone flywheel in one screen. The board should be able to look at this and immediately understand the value prop. |
| **Fallback** | The CSS mockup shows a realistic Pay Anyone flow — usable as-is if real screenshot is delayed |

#### Mockup Position 3: High Yield Savings (Bottom-right, under Act 3 column)

| Property | Specification |
|---|---|
| **Frame type** | Mobile phone frame (iPhone) |
| **Dimensions** | ~220 × 430 px (9:19.5 aspect ratio) |
| **What to replace with** | Screenshot of the Square Banking mobile app showing the High Yield Savings account screen with APY badge, balance, and interest earned |
| **Source owner** | Square Banking — Savings team / Square Financial Services |
| **Framing notes** | Capture the main savings account view. Must show: account balance, APY rate prominently, interest earned. If pre-launch, use a staging/demo environment screenshot. |
| **Launch timing note** | HYS launches mid-May. If this deck is presented before launch, the CSS mockup or a staging screenshot is appropriate. Label as "pre-launch preview" if using non-production UI. |
| **Fallback** | CSS mockup shows representative UI with 3.75% APY, balance, and interest earned |

---

### Slide 3 — Cash App Banking Product Experiences

#### Mockup Position A: Cash App Tag (Center-top)

| Property | Specification |
|---|---|
| **Frame type** | Product photo / illustration (no device frame) |
| **Dimensions** | ~280 × 280 px |
| **What to replace with** | Official Cash App Tag product photo — the physical NFC device. Ideally: the Tag shown tapping against a contactless terminal, or a hero product shot on dark background. |
| **Source owner** | Cash App Hardware team / Cash App Marketing |
| **Framing notes** | Dark background preferred (matches slide). If the Tag is photographed on white, request a dark-background variant or use the CSS illustration. A short video/GIF of the tap-to-pay moment would be even more impactful — the HTML supports replacing the static mockup with a GIF. |
| **Animation note** | The CSS mockup includes a pulsing green glow animation. If using a static photo, consider adding a subtle CSS glow around the image to maintain the visual energy. |
| **Fallback** | CSS/SVG illustration of the Tag with animated green pulse — effective for board context |

#### Mockup Position B: Debit Flex Card (Center-bottom)

| Property | Specification |
|---|---|
| **Frame type** | Card render (no device frame) |
| **Dimensions** | ~300 × 189 px (standard card 1.586:1 ratio) |
| **What to replace with** | Official Debit Flex card render showing the physical card design. Ideally with the debit↔credit toggle concept visualized (if marketing materials exist showing this). |
| **Source owner** | Cash App Card team / Cash App Design |
| **Framing notes** | Dark card on dark background. If the card design is confidential/unreleased, use the CSS mockup. The key visual element is communicating "one card, two modes" — if a real render doesn't convey this, the CSS mockup with the toggle UI may actually be more effective for the board. |
| **Fallback** | CSS card render with debit↔credit toggle — communicates the concept clearly |

---

### Asset Checklist

Use this checklist to track asset collection before the Figma build:

| # | Asset | Owner | Status | Notes |
|---|---|---|---|---|
| 1 | ChAD onboarding screenshot (web, Sole Proprietor) | Square Banking — ChAD | ☐ Needed | Dashboard modal view |
| 2 | Pay Anyone flow screenshot (vendor search + payment confirm) | Square Banking — Bill Pay | ☐ Needed | **HERO ASSET — prioritize** |
| 3 | Square Credit Card render (physical card) | Square Banking — Credit Card | ☐ Needed | For optional use alongside Pay Anyone |
| 4 | High Yield Savings app screenshot (mobile) | Square Banking — Savings / SFS | ☐ Needed | Staging OK if pre-launch |
| 5 | Cash App Tag product photo (dark background) | Cash App Hardware / Marketing | ☐ Needed | Photo or GIF of tap moment |
| 6 | Cash App Tag tap-to-pay video/GIF | Cash App Hardware | ☐ Nice to have | 3-5 second loop |
| 7 | Debit Flex card render | Cash App Card / Design | ☐ Needed | Physical card design |
| 8 | Debit Flex app UI (debit↔credit toggle) | Cash App Card | ☐ Nice to have | In-app toggle screenshot |
| 9 | Digital wallet provisioning screen | Cash App Card | ☐ Nice to have | Apple Pay add-to-wallet flow |
| 10 | Cash App Green membership UI | Cash App Growth | ☐ Nice to have | New membership concept if available |
| 11 | Square Custom Report Builder screenshot | Square Data / Intelligence Platform | ☐ Optional | For appendix if needed |
| 12 | Phone Plans UI mockup | Cash App — Phone Plans | ☐ Nice to have | AT&T plan selection screen |
| 13 | Apex migration dashboard/progress | Cash App Investing | ☐ Optional | Internal migration tracker |

### Integration Instructions for Designer

When replacing CSS mockups with real assets in Figma:

1. **Maintain the frame dimensions** listed above — crop/resize the real screenshot to fit
2. **Keep the dark background context** — if the real screenshot has a light background, place it inside the same frame style (browser frame or phone frame) used in the CSS mockup
3. **Keep the `[REPLACE: ...]` labels** in the working Figma file until final review, then hide/delete them
4. **If an asset isn't available by deck deadline**, the CSS mockup is designed to be presentation-ready — use it as-is
5. **For the Cash App Tag**: if you have video, embed it as a GIF in the Figma prototype for the presentation version. For the static PDF export, use the best still frame.
