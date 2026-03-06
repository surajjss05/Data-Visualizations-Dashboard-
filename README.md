# Data-Visualizations-Dashboard-
# 📊 NexaCorp Analytics — Command Center Dashboard

<div align="center">

![NexaCorp Banner](https://img.shields.io/badge/NexaCorp-Analytics%20Command%20Center-3b82f6?style=for-the-badge&logo=chartdotjs&logoColor=white)

**A fully interactive, Power BI–style Business Intelligence Dashboard built with vanilla HTML, CSS, and JavaScript.**
Real-time KPIs · Revenue Analytics · Deal Pipeline · Sales Forecasting · Team Performance

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-View_Dashboard-10b981?style=for-the-badge)](https://github.com/surajshinde)
[![License](https://img.shields.io/badge/License-MIT-a855f7?style=for-the-badge)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-Pure_Vanilla-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Chart.js](https://img.shields.io/badge/Chart.js-v4.4.1-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)

</div>

---

## 🖼️ Preview

> 🔥 **Single-file dashboard** — No build tools. No frameworks. No installations. Just open `nexacorp_dashboard.html` in any browser and it works.

| 🌙 Dark Theme | ☀️ Light Theme |
|---|---|
| Deep navy design with glowing accents | Clean white with subtle shadows |

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [📊 Dashboard Sections](#-dashboard-sections)
- [🛠️ Tech Stack](#️-tech-stack)
- [🚀 Getting Started](#-getting-started)
- [📁 Project Structure](#-project-structure)
- [🎨 Design System](#-design-system)
- [⚙️ Configuration and Customization](#️-configuration-and-customization)
- [📈 Data Schemas](#-data-schemas)
- [🔧 Functional Features](#-functional-features)
- [🌐 Browser Compatibility](#-browser-compatibility)
- [📱 Responsive Design](#-responsive-design)
- [🤝 Contributing](#-contributing)
- [🗺️ Roadmap](#️-roadmap)
- [📄 License](#-license)
- [👤 Author](#-author)

---

## ✨ Features

### 🎛️ Interactive Controls
- **Period Selector** — Toggle between `1M`, `3M`, `6M`, `YTD`, and `1Y` — all KPI values scale dynamically
- **Multi-Filter System** — Filter by Region, Product Category, and Sales Rep simultaneously
- **Global Search Bar** — Real-time search across the entire deal pipeline table
- **Column Sorting** — Sort deals ascending/descending by deal value with one click
- **Stage Filter Dropdown** — Isolate deals by stage (Proposal, Negotiation, Closed Won, Stalled, etc.)
- **Chart View Toggle** — Switch the revenue trend between Monthly and Quarterly granularity
- **Data Mode Toggle** — Switch the bar chart between Revenue ($) and Units Sold views
- **Refresh Button** — Animated data refresh with spinner feedback and timestamp update
- **Export CSV** — One-click download of the full deals pipeline as a real `.csv` file

### 🌙 Theme and UX
- **Dark / Light Theme Toggle** — Full theme switch; all 8 Chart.js charts re-render in the correct palette
- **Notification Modal** — Slide-in notification center with 4 alert types (revenue, churn, deal won/lost)
- **Sidebar Tooltips** — Smooth animated labels appear on sidebar icon hover
- **Animated KPI Counters** — Values animate on load with staggered entrance delays per card
- **Micro-interactions** — Hover lifts, glow borders, and active highlights on every interactive element
- **Live Badge** — Pulsing animated "Live" indicator in the header
- **Background Mesh** — Floating radial-gradient orbs create subtle visual depth

### 📊 Visualizations (8 Chart Types)
- 📈 **Multi-line Area Chart** — Revenue, Profit, and Target trend with crosshair tooltips
- 🍩 **Donut Chart** — Revenue by sales channel with custom inline legend
- 📊 **Horizontal Bar Chart** — Sales by product category (Revenue or Units mode)
- 🫧 **Bubble / Scatter Chart** — Deal size vs. win rate correlation matrix
- 🔻 **Sales Funnel** — Animated gradient pipeline conversion waterfall
- 🌡️ **SVG Gauge Meter** — Quota attainment with animated rotating needle and gradient arc
- 🗓️ **Activity Heatmap** — GitHub-style 12-month daily activity contribution calendar
- ✨ **Sparkline KPI Cards** — 4 live mini trend charts at the bottom (Conversion, Churn, NPS, LTV)

---

## 📊 Dashboard Sections

### 1️⃣ KPI Summary Row
Four top-level metric cards:

| Metric | Value | YoY Change |
|--------|-------|------------|
| 💰 Total Revenue | $48.7M | ▲ +18.4% |
| 🛒 Total Orders | 124,830 | ▲ +9.2% |
| 👤 Active Customers | 38,410 | ▲ +6.7% |
| 📦 Avg Order Value | $390 | ▼ -2.1% |

Each card includes a mini sparkline, trend badge, color-coded stripe, and click-to-highlight interaction.

### 2️⃣ Revenue and Profit Trend (Line Chart)
- Monthly or quarterly toggle for Revenue, Profit, and Target lines
- Inline stat pills: total revenue, total profit, and gross margin %
- Unified crosshair tooltip showing all three series simultaneously

### 3️⃣ Revenue by Channel (Donut Chart)

| Channel | Share | Value |
|---------|-------|-------|
| Direct Sales | 38% | $18.5M |
| Online / Ecom | 27% | $13.1M |
| Partners | 22% | $10.7M |
| Resellers | 13% | $6.4M |

### 4️⃣ Sales by Product Category (Bar Chart)
Horizontal bar comparison across Software, Hardware, Services, Consulting, and Training — togglable between Revenue ($M) and Units Sold.

### 5️⃣ Sales Funnel
Stage-by-stage animated conversion: Leads (4,820) → Qualified → Proposal → Negotiation → Closed Won (186).

### 6️⃣ Top Sales Representatives
Ranked leaderboard of 6 reps with avatar, territory/role, revenue vs target, attainment %, and color bar.

### 7️⃣ Active Deal Pipeline (Table)
8-row table with: client name, deal value, stage, rep, probability bar, win %, and status chip — filterable, sortable, and searchable.

### 8️⃣ Quota Attainment Gauge
SVG arc meter (0–100%) with animated needle pointing to 74.9% and a gradient track from red → amber → green.

### 9️⃣ Deal Size vs Win Rate (Bubble Chart)
Scatter plot correlating avg deal size ($K) with win rate (%), bubble size = deal volume per product category.

### 🔟 Activity Heatmap Calendar
GitHub-style contribution grid at 5 intensity levels (L0–L4) per week across all 12 months.

### 1️⃣1️⃣ Live KPI Sparklines (Bottom Row)
Four metric cards with full-width sparkline trends:
- Conversion Rate → 24.6%
- Churn Rate → 3.2%
- NPS Score → 72
- Customer LTV → $1,840

---

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) **HTML5** | 5 | Semantic document structure and layout |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) **CSS3** | 3 | Custom design system, animations, dual-theme engine |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) **Vanilla JavaScript** | ES2020+ | All interactivity, DOM rendering, state management |
| ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white) **Chart.js** | 4.4.1 | All 8 chart types: line, bar, doughnut, bubble, sparkline |
| ![Google Fonts](https://img.shields.io/badge/Google_Fonts-4285F4?style=flat-square&logo=googlefonts&logoColor=white) **Google Fonts** | — | `Outfit` (UI font) + `JetBrains Mono` (data values) |
| ![SVG](https://img.shields.io/badge/SVG-FFB13B?style=flat-square) **Inline SVG** | — | Custom animated gauge with rotating needle |
| ![CSS Variables](https://img.shields.io/badge/CSS_Custom_Properties-8b5cf6?style=flat-square) **CSS Custom Properties** | — | Dual-theme system toggled via `data-theme` attribute |
| ![Cloudflare CDN](https://img.shields.io/badge/Cloudflare_CDN-F38020?style=flat-square&logo=cloudflare&logoColor=white) **Cloudflare CDN** | — | Chart.js delivery from `cdnjs.cloudflare.com` |
| ![CSS Grid](https://img.shields.io/badge/CSS_Grid_&_Flexbox-1572B6?style=flat-square) **CSS Grid + Flexbox** | — | Responsive multi-column adaptive layout system |

### 🏗️ Architecture Highlights

- **Zero build tools** — No Webpack, Vite, Rollup, Parcel, or any bundler
- **Zero backend** — 100% client-side; works offline after initial CDN font/script load
- **Zero npm packages** — No `package.json`, no `node_modules`, just one `<script>` CDN tag
- **CSS-only motion** — `@keyframes`, `transition`, and `transform` handle all animations
- **CSS Custom Properties** — 20+ theme tokens in `:root`, switched with `data-theme="light"` on `<html>`
- **Chart.js lifecycle management** — Charts are destroyed and recreated on theme toggle for correct palette application
- **Modular JS renderer functions** — Each section has an isolated `renderX()` function for easy maintenance and extension

---

## 🚀 Getting Started

### ✅ Prerequisites

**None.** Zero local dependencies. You only need a modern web browser.

### 📥 Installation

**Option 1 — Clone with Git:**
```bash
git clone https://github.com/surajshinde/nexacorp-analytics-dashboard.git
cd nexacorp-analytics-dashboard
```

**Option 2 — Download the single file:**
```bash
curl -O https://raw.githubusercontent.com/surajshinde/nexacorp-analytics-dashboard/main/nexacorp_dashboard.html
```

**Option 3 — GitHub ZIP:**
> Click the green **Code** button → **Download ZIP** → Extract → Open `nexacorp_dashboard.html`

### ▶️ Running the Dashboard

**Simplest — just open in browser:**
```bash
open nexacorp_dashboard.html          # macOS
start nexacorp_dashboard.html         # Windows
xdg-open nexacorp_dashboard.html      # Linux
```

**Or use a local HTTP server:**
```bash
# Python (zero install)
python3 -m http.server 8080

# Node.js (zero install via npx)
npx serve .

# VS Code — use the "Live Server" extension
```

Then open: **`http://localhost:8080/nexacorp_dashboard.html`**

> 💡 Best viewed at **1280px+ screen width** for the full multi-column layout experience.

---

## 📁 Project Structure

```
nexacorp-analytics-dashboard/
│
├── 📄 nexacorp_dashboard.html   ← Complete dashboard (self-contained single file)
├── 📄 README.md                 ← Project documentation (you are here)
└── 📄 LICENSE                   ← MIT License
```

> **Single-file architecture** — All HTML structure, CSS styling, and JavaScript logic live inside one `.html` file. Share one file and it works anywhere with a browser — no server, no setup.

---

## 🎨 Design System

### 🎨 Color Palette

| Token | Dark Value | Light Value | Usage |
|-------|-----------|-------------|-------|
| `--bg` | `#070b14` | `#f0f4fc` | Page background |
| `--panel` | `#0f1523` | `#ffffff` | Card and panel surfaces |
| `--panel2` | `#141d2e` | `#f7f9ff` | Hover and nested backgrounds |
| `--border` | `rgba(255,255,255,0.07)` | `rgba(0,0,0,0.07)` | Subtle card borders |
| `--a1` | `#3b82f6` | `#3b82f6` | Primary accent — Blue |
| `--a2` | `#a855f7` | `#a855f7` | Secondary accent — Purple |
| `--a3` | `#10b981` | `#10b981` | Success / Positive — Emerald |
| `--a4` | `#f59e0b` | `#f59e0b` | Warning — Amber |
| `--a5` | `#ef4444` | `#ef4444` | Danger / Negative — Red |
| `--a6` | `#06b6d4` | `#06b6d4` | Info — Cyan |
| `--pos` | `#10b981` | `#10b981` | Positive delta badge |
| `--neg` | `#ef4444` | `#ef4444` | Negative delta badge |

### 🔤 Typography

| Font | Weights | Role |
|------|---------|------|
| **Outfit** | 300–900 | All UI text: labels, buttons, headings, body |
| **JetBrains Mono** | 400, 500 | KPI numeric values for precise tabular alignment |

### 📐 Spacing and Geometry
- Base unit: `4px`
- Card `border-radius`: `16px`
- Button `border-radius`: `8–10px`
- Badge / chip `border-radius`: `20px` (full pill)
- Content padding: `24px 28px`

### 🎞️ Motion Design

| Animation | Technique |
|-----------|-----------|
| Page load entrance | `@keyframes fadeUp` with staggered `animation-delay` per component |
| Card hover lift | `transform: translateY(-4px)` + `box-shadow` glow via `transition` |
| Theme crossfade | `transition: background 0.4s ease` on all color-bearing elements |
| Notification pulse | `@keyframes pulse` scale oscillation on dots and badges |
| SVG gauge needle | `transform: rotate()` via CSS `transition` |
| Funnel bar fill | CSS `width` transition with `cubic-bezier(.4,0,.2,1)` timing |
| Background orbs | `@keyframes meshFloat` continuous translate + scale loop |

---

## ⚙️ Configuration and Customization

### 🔄 Updating KPI Cards

Edit the `KPI_DATA` array in the `<script>` section:

```javascript
const KPI_DATA = [
  {
    id:     'rev',
    label:  'Total Revenue',
    value:  48.7,           // Numeric value to display
    unit:   '$',            // Prefix: '$' or '' for none
    suffix: 'M',            // Suffix: 'M', 'K', or ''
    change: +18.4,          // YoY percentage change
    dir:    'up',           // 'up' or 'down'
    color:  'var(--a1)',    // CSS color variable for accent
    colorG: 'var(--a1g)',   // CSS color variable (glass variant)
    icon:   '💰',           // Emoji for icon box
    spark:  [2.8, 3.1, ...] // 12-point array for mini sparkline
  },
];
```

### 📅 Revenue Trend Data

```javascript
const DATA = {
  monthly: {
    labels:  ['Jan','Feb','Mar', ...],  // 12 month labels
    revenue: [2.8, 3.1, 3.4, ...],     // Revenue in $M per month
    profit:  [0.9, 1.0, 1.1, ...],     // Profit in $M per month
    target:  [3.0, 3.2, 3.5, ...],     // Target in $M per month
  },
  quarterly: {
    labels:  ['Q1 2024','Q2 2024','Q3 2024','Q4 2024'],
    revenue: [9.3, 11.8, 13.0, 14.6],
    profit:  [3.0,  4.1,  4.8,  4.7],
    target:  [9.7, 12.2, 14.0, 15.6],
  }
};
```

### 🤝 Deal Pipeline Entries

```javascript
const DEALS = [
  {
    rank:   1,
    client: 'Apex Technologies',
    value:  2400000,         // Deal value in USD (integer)
    stage:  'Proposal',      // Must match filter dropdown labels
    rep:    'Sarah K.',      // Sales rep display name
    prob:   75,              // Win probability 0–100 (drives bar color)
    status: 'live'           // 'live' | 'pend' | 'won' | 'lost'
  },
];
```

### 👥 Sales Rep Leaderboard

```javascript
const REPS = [
  {
    name:     'Sarah K.',
    role:     'Enterprise',
    rev:      8.2,           // Revenue achieved in $M
    target:   9.0,           // Annual target in $M (drives % bar)
    color:    '#3b82f6',     // Hex color for avatar and bar fill
    initials: 'SK'           // 2-char initials for avatar circle
  },
];
```

### 🌈 Overriding the Color Scheme

All tokens are CSS custom properties in `:root`. Override any of them:

```css
:root {
  --a1: #your-primary-color;   /* Replace blue accent */
  --a2: #your-secondary-color; /* Replace purple accent */
  --a3: #your-success-color;   /* Replace emerald */
  --bg: #your-dark-bg;         /* Replace dark background */
}
```

---

## 📈 Data Schemas

### Deal Interface
```typescript
interface Deal {
  rank:   number;
  client: string;
  value:  number;   // USD integer
  stage:  'Prospecting' | 'Proposal' | 'Negotiation' | 'Closed Won' | 'Stalled';
  rep:    string;
  prob:   number;   // 0–100
  status: 'live' | 'pend' | 'won' | 'lost';
}
```

### Sales Rep Interface
```typescript
interface SalesRep {
  name:     string;
  role:     string;   // Territory segment
  rev:      number;   // Revenue achieved in $M
  target:   number;   // Annual target in $M
  color:    string;   // Hex color string
  initials: string;   // 2-character initials
}
```

### KPI Card Interface
```typescript
interface KPI {
  id:      string;
  label:   string;
  value:   number;
  unit:    string;          // '$' or ''
  suffix:  string;          // 'M', 'K', or ''
  change:  number;          // YoY % (positive or negative)
  dir:     'up' | 'down';
  color:   string;          // CSS variable
  colorG:  string;          // CSS variable (glass variant)
  icon:    string;          // Emoji string
  spark:   number[];        // 12-point sparkline array
}
```

---

## 🔧 Functional Features

### 🔍 Global Search
Real-time search filters the deal table on:
- **Client name** (partial match, case-insensitive)
- **Sales rep name** (partial match)
- **Pipeline stage** (partial match)

Result count label updates dynamically. Clear the input to restore the full table.

### 📤 CSV Export
The **⬇ Export CSV** button generates and immediately downloads a real file using the browser's native `Blob` + `<a download>` API — no server required:

```
Client,Value,Stage,Rep,Probability,Status
Apex Technologies,2400000,Proposal,Sarah K.,75%,live
GlobalNet Corp,1900000,Negotiation,Mark D.,88%,live
...
```

### 🌗 Dark / Light Theme Toggle
- Clicking 🌙 / 🌞 toggles `data-theme` on `<html>` between `"dark"` and `"light"`
- All 8 Chart.js chart instances are destroyed and re-instantiated with theme-aware colors
- Every color surface uses CSS custom properties — transition is complete and seamless

### 🔔 Notification Center
Click 🔔 to open the modal overlay containing 4 categorized alert cards:
- 📈 Revenue milestone reached (blue)
- ⚠️ Churn risk alert (amber)
- ✅ Deal closed (green)
- ❌ Deal lost (red)

Click outside the modal or press ✕ to dismiss.

### ↻ Data Refresh Simulation
- Spinner icon animates for 1.2s during simulated reload
- Line chart and heatmap re-render with slightly randomized values
- Footer "last refreshed" timestamp resets to "just now"

### 📅 Period Scaling

| Period Tab | Scale Factor Applied |
|------------|---------------------|
| 1M | ×0.42 |
| 3M | ×0.75 |
| 6M | ×0.90 |
| YTD | ×1.00 (baseline) |
| 1Y | ×1.05 |

---

## 🌐 Browser Compatibility

| Browser | Min Version | Status |
|---------|------------|--------|
| ![Chrome](https://img.shields.io/badge/Chrome-4285F4?style=flat-square&logo=googlechrome&logoColor=white) Chrome | 90+ | ✅ Full support |
| ![Firefox](https://img.shields.io/badge/Firefox-FF7139?style=flat-square&logo=firefox&logoColor=white) Firefox | 88+ | ✅ Full support |
| ![Safari](https://img.shields.io/badge/Safari-000000?style=flat-square&logo=safari&logoColor=white) Safari | 14+ | ✅ Full support |
| ![Edge](https://img.shields.io/badge/Edge-0078D7?style=flat-square&logo=microsoftedge&logoColor=white) Edge | 90+ | ✅ Full support |
| ![Opera](https://img.shields.io/badge/Opera-FF1B2D?style=flat-square&logo=opera&logoColor=white) Opera | 76+ | ✅ Full support |
| Internet Explorer | Any | ❌ Not supported |

> ⚠️ Internet Explorer is unsupported due to use of CSS Custom Properties, `backdrop-filter`, ES2020 syntax, and CSS Grid.

---

## 📱 Responsive Design

| Breakpoint | Layout Behavior |
|-----------|----------------|
| `> 1200px` | 4-column KPI row + full multi-column chart rows |
| `768px – 1200px` | 2-column KPI row + stacked/2-column chart rows |
| `< 768px` | Single column, sidebar hidden, condensed padding |

CSS Grid with `grid-template-columns` and `@media` breakpoints handles all responsive behavior — no JavaScript involved in layout switching.

---

## 🤝 Contributing

Contributions, issues, and feature requests are very welcome!

### 🐛 Bug Reports
Open an issue titled: `[BUG] Short description`
- Include browser, OS, screen resolution
- Describe expected vs actual behavior
- Attach a screenshot if helpful

### 💡 Feature Requests
Open an issue titled: `[FEATURE] Short description`
- Describe the use case and the value it adds

### 🔀 Pull Request Process

```bash
# 1. Fork this repo on GitHub
# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/nexacorp-analytics-dashboard.git

# 3. Create your feature branch
git checkout -b feature/your-feature-name

# 4. Make changes to nexacorp_dashboard.html
# 5. Test in at least Chrome and Firefox

# 6. Commit with a conventional message
git add .
git commit -m "✨ feat: brief description of your change"

# 7. Push and open a Pull Request
git push origin feature/your-feature-name
```

### 📝 Commit Conventions

```
✨ feat:      New feature
🐛 fix:       Bug fix
🎨 style:     CSS / design changes
📊 data:      Data or schema updates
📝 docs:      README or documentation
⚡ perf:      Performance improvement
♻️  refactor:  Code restructure, no behavior change
🔧 config:    Configuration changes
```

---

## 🗺️ Roadmap

- [ ] 🔌 REST API / WebSocket integration for live data fetching
- [ ] 💾 `localStorage` persistence for filter preferences and theme choice
- [ ] 🖨️ Print / PDF export of the full dashboard layout
- [ ] 📧 Scheduled email report UI mockup
- [ ] 🗺️ Interactive world map with Leaflet.js for regional drill-down
- [ ] 📅 Custom date range picker component
- [ ] 🧮 Calculated KPI formula editor
- [ ] 🔐 Role-based view modes (Executive / Sales / Finance)
- [ ] 🧩 Drag-and-drop widget grid for custom card arrangement
- [ ] 🌍 i18n / localization (currency formats, date formats, languages)

---

## 📄 License

```
MIT License

Copyright (c) 2024 Suraj Shinde

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

See the [LICENSE](LICENSE) file for full details.

---

## 👤 Author

<div align="center">

### **Suraj Shinde**

[![GitHub](https://img.shields.io/badge/GitHub-@surajshinde-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/surajshinde)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Suraj_Shinde-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/surajshinde)
[![Portfolio](https://img.shields.io/badge/Portfolio-surajshinde.dev-3b82f6?style=for-the-badge&logo=vercel&logoColor=white)](https://surajshinde.dev)
[![Email](https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:suraj@surajshinde.dev)

*"Building beautiful, data-driven interfaces that make complex information instantly understandable."*

</div>

---

## 🌟 Show Your Support

If this project helped you or you found it useful:

- ⭐ **Star** this repository
- 🍴 **Fork** it as the base for your own dashboard
- 📢 **Share** it with developers and data teams in your network
- 🐛 **Contribute** bug reports, features, or pull requests

---

<div align="center">

**Made with ❤️ and ☕ by [Suraj Shinde](https://github.com/surajshinde)**

![Visitors](https://img.shields.io/badge/Visitors-Welcome-10b981?style=flat-square)
![Maintained](https://img.shields.io/badge/Maintained-Yes-3b82f6?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-a855f7?style=flat-square)
![Zero Dependencies](https://img.shields.io/badge/Zero_Dependencies-Single_File-f59e0b?style=flat-square)

</div>
