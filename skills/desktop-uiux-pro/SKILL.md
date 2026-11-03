---
name: desktop-uiux-pro
description: Elite Desktop UI/UX Design System & Product Design skill. Synthesized from 170+ high-converting B2B SaaS platforms, analytics dashboards, and agency references. Guides any AI to architect modern Bento grids, dense enterprise data tables, NeoSoftUI dark mode systems, high-converting SaaS landing pages, keyboard shortcut navigation, and production-ready desktop Tailwind CSS code.
---

# Desktop UI/UX Pro Designer (Agent Skill)

> **Universal AI Compatibility**: This skill works natively with **Claude, ChatGPT / GPT-4o, Gemini, Cursor, Windsurf, Antigravity, Copilot, Cline, and any LLM agent**.

A masterclass design system and frontend engineering methodology distilled from analyzing 170+ professional desktop SaaS interfaces, analytics portals, and agency portfolios (@webdesignssphere, @siren.uix, @webstarinfotech, @deluxewebsite).

---

## 🖥️ Core Behavioral Directives for the AI

When the user asks you to design or code a desktop web application, SaaS platform, or widescreen landing page, you MUST embody the role of a **Principal Desktop Product Architect & Frontend Systems Engineer**. Always enforce these 5 foundational desktop laws:

### 1. Spatial Density & The 3-Tier Desktop Layout
Unlike mobile interfaces that demand single-column focus, desktop users require high information density without unnecessary pagination:
- **Left Tier (Navigation Bar)**: Compact collapsible sidebar (64px collapsed icon-only / 240px expanded) with workspace switcher and keyboard hotkeys.
- **Top Tier (Context & Command Bar)**: Global search (`⌘K` Command Palette), breadcrumbs, active workspace indicator, and user profile drawer.
- **Main Viewport (The Work Surface)**: Asymmetric Bento Grid or dense multi-metric data canvases utilizing minimum 12-column or fluid CSS grids (`gap-6`).

### 2. Proof Precedes Pitch (Conversion Architecture)
In B2B SaaS and high-ticket desktop landing pages:
- Social proof (Logo cloud of recognizable tech brands, rating stars, live active telemetry numbers) MUST appear **above the fold** or directly underneath the hero headline before explaining complex product features.
- Pair abstract product claims with a **Floating Interactive Mockup** (isometric 3D tilt, realistic metric badges, and active trend indicators).
- Maintain a strict **3-Beat Scan Rhythm**: Headline + 3 Bullet Points + 1 Explicit CTA Button.

### 3. NeoSoftUI Desktop Aesthetics (Motvin System)
Derived from `@siren.uix` Motvin Design principles:
- **Canvas Base (60%)**: Deep layered obsidian (`#06090F`, `#0B0F17`, `#121824`). Avoid pure `#000000` to preserve depth and separation.
- **Surface Elevation (30%)**: Glassmorphic cards with:
  ```css
  background: rgba(16, 22, 35, 0.65);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.08);
  box-shadow: 0 20px 45px -10px rgba(0, 0, 0, 0.5), inset 0 1px 0 rgba(255, 255, 255, 0.08);
  ```
- **High-Impact Accent (10%)**: Electric Indigo (`#6366F1`) or Cyan Neon (`#06B6D4`) reserved exclusively for primary buttons, active tabs, and telemetry spikes.

### 4. Interactive States & Keyboard Ergonomics
Desktop interfaces live and die by mouse precision and keyboard speed:
- **Card Hover Transitions**: Smooth elevation `hover:-translate-y-1 hover:border-indigo-500/40 hover:shadow-indigo-500/10` with 250ms cubic-bezier timing.
- **Floating Batch Action Bar**: When a user selects 2 or more rows in a data table, render a docked floating pill bar at the bottom center (`fixed bottom-8 left-1/2 -translate-x-1/2`) showing actions like *Export CSV*, *Tag Batch*, or *Delete*.
- **Tooltips**: Include keyboard shortcuts in hover tooltips (e.g., `⌘K`, `/`, `Shift + D`).

### 5. Desktop Typography & Information Hierarchy
| Hierarchy Level | Font Size | Weight | Tracking | Usage |
| :--- | :--- | :--- | :--- | :--- |
| **Hero Display** | 56px – 72px | ExtraBold (800) | `-0.025em` (Tight) | Landing page above-the-fold value prop |
| **Page / Section H1**| 32px – 40px | Bold (700) | `-0.02em` | Dashboard view title, Section headers |
| **Widget / Card H2** | 18px – 22px | SemiBold (600) | `-0.01em` | Bento card headings, Table title |
| **Data Metric / Value**| 28px – 36px | ExtraBold (800) | Normal | Key stats, ARR metrics, Counter figures |
| **Body / Description** | 14px – 16px | Regular (400) | Normal | Paragraphs, documentation (1.6 line height) |
| **Code / Monospace** | 12px – 13px | Medium (500) | Normal | Query latency, API endpoints, JSON keys |

---

## 🧩 Production-Ready Desktop Component Blueprints

### Blueprint A: Modern Bento Grid Matrix (Asymmetric Spans)
```html
<div class="grid grid-cols-1 lg:grid-cols-3 gap-6 max-w-7xl mx-auto">
  <!-- Card 1: 2-Column Hero Card (Data Telemetry) -->
  <div class="lg:col-span-2 rounded-2xl border border-white/10 bg-[#101623]/80 p-8 backdrop-blur-xl relative overflow-hidden group hover:border-indigo-500/40 transition-all duration-300">
    <!-- Ambient Radial Glow -->
    <div class="absolute -right-20 -top-20 h-64 w-64 rounded-full bg-indigo-500/10 blur-3xl group-hover:bg-indigo-500/20 transition-all"></div>
    
    <div class="flex items-center justify-between mb-6">
      <div class="flex items-center gap-3">
        <div class="h-10 w-10 rounded-xl bg-indigo-500/10 border border-indigo-500/20 text-indigo-400 flex items-center justify-center font-bold">⚡</div>
        <div>
          <h3 class="text-xl font-bold text-white">Sub-Second Query Pipeline</h3>
          <p class="text-xs text-neutral-400">ClickHouse columnar storage engine</p>
        </div>
      </div>
      <span class="px-2.5 py-1 rounded-md bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 text-xs font-mono">P99: 11.2ms</span>
    </div>

    <p class="text-sm text-neutral-300 max-w-xl leading-relaxed mb-6">
      Scan through billions of telemetry logs without pre-aggregation bottlenecks. Isolate customer drop-offs with zero cold starts.
    </p>

    <!-- Visual Sparkline Simulation -->
    <div class="h-28 rounded-xl bg-black/40 border border-white/5 p-4 flex items-end gap-3 justify-between">
      <div class="w-full bg-neutral-800 rounded h-[40%]"></div>
      <div class="w-full bg-neutral-800 rounded h-[55%]"></div>
      <div class="w-full bg-neutral-800 rounded h-[45%]"></div>
      <div class="w-full bg-indigo-900/60 rounded h-[70%]"></div>
      <div class="w-full bg-gradient-to-t from-indigo-600 to-cyan-400 rounded h-[95%] relative">
        <span class="absolute -top-7 left-1/2 -translate-x-1/2 text-[10px] font-mono font-bold text-white bg-indigo-900 px-2 py-0.5 rounded border border-indigo-500/30">+32%</span>
      </div>
      <div class="w-full bg-indigo-500 rounded h-[75%]"></div>
    </div>
  </div>

  <!-- Card 2: 1-Column Metric Card -->
  <div class="rounded-2xl border border-white/10 bg-[#101623]/80 p-8 backdrop-blur-xl flex flex-col justify-between group hover:border-cyan-500/40 transition-all duration-300">
    <div>
      <span class="text-xs font-mono font-bold uppercase tracking-wider text-cyan-400">Retention Shield</span>
      <h3 class="text-lg font-bold text-white mt-2">Autonomous Churn Alert</h3>
      <p class="text-xs text-neutral-400 mt-1 leading-relaxed">Continuous ML monitoring detects anomalies before renewal dates.</p>
    </div>
    <div class="my-6">
      <div class="text-5xl font-extrabold tracking-tight text-white">$482<span class="text-2xl text-cyan-400 font-normal">k</span></div>
      <p class="text-xs text-neutral-500 mt-1">ARR preserved via proactive interventions</p>
    </div>
    <div class="flex items-center gap-1.5 text-xs font-semibold text-cyan-400 group-hover:translate-x-1 transition-transform">
      <span>Configure webhook triggers</span> →
    </div>
  </div>
</div>
```

---

### Blueprint B: Dense Enterprise Data Table with Floating Batch Bar
```html
<div class="rounded-2xl border border-white/10 bg-[#0B0F17] overflow-hidden text-sm">
  <!-- Table Header Actions -->
  <div class="p-5 border-b border-white/5 flex items-center justify-between bg-[#101623]/60">
    <div class="flex items-center gap-3">
      <h3 class="font-bold text-white">Live Telemetry Events</h3>
      <span class="px-2 py-0.5 rounded bg-white/5 text-neutral-400 text-xs font-mono">1,420,892 total</span>
    </div>
    <div class="flex items-center gap-2">
      <input type="text" placeholder="Filter by event name, user ID, region..." class="px-3 py-1.5 rounded-lg bg-black/40 border border-white/10 text-xs text-white placeholder-neutral-500 focus:outline-none focus:border-indigo-500 w-64"/>
      <button class="px-3 py-1.5 rounded-lg border border-white/10 bg-white/5 hover:bg-white/10 text-xs text-neutral-300 font-medium">Export CSV</button>
    </div>
  </div>

  <!-- Table Body -->
  <table class="w-full text-left border-collapse">
    <thead>
      <tr class="border-b border-white/5 text-xs font-mono text-neutral-400 bg-white/[0.01]">
        <th class="p-4 w-10"><input type="checkbox" class="rounded bg-black border-white/20"/></th>
        <th class="p-4">Timestamp</th>
        <th class="p-4">Event Type</th>
        <th class="p-4">Customer Account</th>
        <th class="p-4">Ingestion Latency</th>
        <th class="p-4 text-right">Status</th>
      </tr>
    </thead>
    <tbody class="divide-y divide-white/5 text-neutral-300 text-xs font-mono">
      <tr class="hover:bg-white/[0.02] transition-colors">
        <td class="p-4"><input type="checkbox" class="rounded bg-black border-white/20"/></td>
        <td class="p-4 text-neutral-400">10:42:01.412 UTC</td>
        <td class="p-4 font-semibold text-white">checkout.payment_confirmed</td>
        <td class="p-4 font-sans text-neutral-200">Stripe Billing Cluster #4</td>
        <td class="p-4 text-emerald-400">6.2 ms</td>
        <td class="p-4 text-right"><span class="px-2 py-0.5 rounded bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 text-[10px]">PROCESSED</span></td>
      </tr>
      <tr class="hover:bg-white/[0.02] transition-colors">
        <td class="p-4"><input type="checkbox" class="rounded bg-black border-white/20"/></td>
        <td class="p-4 text-neutral-400">10:41:58.204 UTC</td>
        <td class="p-4 font-semibold text-white">user.invitation_accepted</td>
        <td class="p-4 font-sans text-neutral-200">Acme Corp Enterprise</td>
        <td class="p-4 text-emerald-400">8.4 ms</td>
        <td class="p-4 text-right"><span class="px-2 py-0.5 rounded bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 text-[10px]">PROCESSED</span></td>
      </tr>
    </tbody>
  </table>

  <!-- Floating Docked Batch Action Bar (Appears when 2+ rows checked) -->
  <div class="fixed bottom-8 left-1/2 -translate-x-1/2 px-5 py-3 rounded-2xl bg-[#172033] border border-indigo-500/40 shadow-2xl shadow-black/80 flex items-center gap-4 text-xs z-50">
    <span class="font-semibold text-white"><span class="text-indigo-400 font-mono">2</span> items selected</span>
    <div class="h-4 w-px bg-white/10"></div>
    <button class="text-neutral-300 hover:text-white font-medium">Re-run Pipeline</button>
    <button class="text-neutral-300 hover:text-white font-medium">Export JSON</button>
    <button class="text-rose-400 hover:text-rose-300 font-medium">Purge Records</button>
  </div>
</div>
```

---

## 🚫 Desktop Anti-Patterns (Do's and Don'ts)

| NEVER DO THIS (Anti-Pattern) | ALWAYS DO THIS (Desktop Best Practice) |
| :--- | :--- |
| Stretches a single-column mobile layout across 1920px. | Use multi-column Bento grids or multi-pane master-detail layouts. |
| Forcing users to paginate data tables at only 5 rows per page. | Default to 25–50 rows with sticky table headers and instant search filtering. |
| Using pure `#000000` backgrounds with harsh `#FFFFFF` borders. | Layer deep obsidians (`#0B0F17`) with subtle glassmorphic borders (`border-white/10`). |
| Hiding keyboard shortcuts from advanced enterprise users. | Display shortcut tags (`⌘K`, `/`, `G then D`) directly on interactive elements. |
| Relying on slow full-page reloads for simple state filters. | Update telemetry charts and table rows instantaneously via optimistic UI updates. |

---

## 💬 AI Prompting Templates (How Users Can Prompt You)

Users can activate this skill by prompting:
- *"Using the `desktop-uiux-pro` skill, design an enterprise analytics dashboard with a Bento grid and live ClickHouse telemetry tables."*
- *"Using `desktop-uiux-pro`, architect a B2B SaaS landing page with NeoSoftUI dark mode, proof-before-pitch, and a 3-tier pricing matrix."*
- *"Review this desktop layout for spatial density, keyboard shortcuts, and WCAG contrast."*
