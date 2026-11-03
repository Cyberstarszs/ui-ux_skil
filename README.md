# 🎨 Universal UI/UX AI Skills — Mobile & Desktop Pro

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Agent Skills Specification](https://img.shields.io/badge/Agent%20Skills-v1.0%20Compatible-indigo.svg)](https://skills.sh)
[![Multi-AI Support](https://img.shields.io/badge/Supports-Claude%20%7C%20ChatGPT%20%7C%20Cursor%20%7C%20Gemini%20%7C%20Windsurf-emerald.svg)](#-how-to-use-with-any-ai)
[![Dataset](https://img.shields.io/badge/Curated%20Dataset-950%2B%20Analyzed%20Screens-purple.svg)](#-empirical-data-foundation)

> **Two battle-tested, production-grade AI Skills designed to transform any AI coding assistant into a Principal Product Designer & Frontend Architect.**  
> Distilled and empirically synthesized from over **950+ curated professional UI/UX reference screens** from elite product designers and digital agencies (@webdesignssphere, @siren.uix, @webstarinfotech, @deluxewebsite).

---

## 📦 What's Inside

| Skill Name | Path | Primary Domain | Key Methodologies |
| :--- | :--- | :--- | :--- |
| **`mobile-uiux-pro`** | [`.agents/skills/mobile-uiux-pro/SKILL.md`](.agents/skills/mobile-uiux-pro/SKILL.md) | iOS & Android Mobile Apps | Thumb Zone reachability, "Rule of One" onboarding, Swipeable Bottom Sheets, OLED true-dark palettes, 48px touch targets, Safe Area ergonomics. |
| **`desktop-uiux-pro`** | [`.agents/skills/desktop-uiux-pro/SKILL.md`](.agents/skills/desktop-uiux-pro/SKILL.md) | B2B SaaS & Desktop Web Apps | NeoSoftUI dark mode, Asymmetric Bento grids, Dense enterprise data tables, Keyboard shortcuts (`⌘K`), Floating multi-select batch bars, Proof-before-pitch. |

---

## ⚡ How to Use with ANY AI

These skills follow the open **Agent Skills Specification** and standard Markdown, making them **100% compatible with every modern AI tool**.

### 1. Antigravity / Agent Skills CLI
If you are using Antigravity or the `skills` CLI:
```bash
# Skills are automatically loaded if in .agents/skills/
npx skills add .agents/skills/mobile-uiux-pro
npx skills add .agents/skills/desktop-uiux-pro
```

### 2. Cursor IDE
- Create `.cursor/rules/mobile-uiux.mdc` and paste the contents of [`mobile-uiux-pro/SKILL.md`](.agents/skills/mobile-uiux-pro/SKILL.md).
- Create `.cursor/rules/desktop-uiux.mdc` and paste the contents of [`desktop-uiux-pro/SKILL.md`](.agents/skills/desktop-uiux-pro/SKILL.md).
- *Or simply paste into your root `.cursorrules` file.*

### 3. Claude (Claude Desktop, Claude Code & Projects)
- In **Claude Projects**, go to **Project Knowledge** and upload both `SKILL.md` files.
- In **Claude Code CLI**, reference them directly in your project prompt:
  ```bash
  claude "Using the mobile-uiux-pro skill, design a crypto wallet onboarding flow"
  ```

### 4. ChatGPT / OpenAI (Custom GPTs)
- Go to [chatgpt.com/gpts/editor](https://chatgpt.com/gpts/editor).
- In the **Instructions** box, copy and paste either `mobile-uiux-pro/SKILL.md` or `desktop-uiux-pro/SKILL.md`.
- Now your custom GPT will exclusively design world-class interfaces following these rules!

### 5. Windsurf / Cascade (Codeium)
- Add the skills into your `.windsurfrules` file or drop them into your project root.

### 6. Cline / Roo Code / Copilot
- Include the `SKILL.md` file in `.clinerules` or attach it to your context when prompting.

---

## 📱 1. `mobile-uiux-pro` Highlights

### The 5 Laws of Mobile UI/UX:
1. **The Thumb Zone Rule**: The bottom 35% of the mobile viewport is the primary action zone. Primary CTAs, tab bars, and confirmations must reside here.
2. **"The Rule of One" Onboarding**: Wellness and fintech apps drop 70% of users during registration. Exactly **one user decision per screen** using tappable cards/chips instead of intimidating form fields.
3. **Swipeable Bottom Sheets**: Replaces desktop modals with native bottom sheets (`rounded-t-[32px]`) featuring top drag handles and safe area margins.
4. **OLED Dark Mode**: True dark canvas (`#090A0F`) with subtle `#12151F` elevated cards for high contrast and battery efficiency.
5. **Touch Targets**: Minimum 48x48px interactive target bounds with 8px clearance.

👉 **View Full Mobile Skill**: [`.agents/skills/mobile-uiux-pro/SKILL.md`](.agents/skills/mobile-uiux-pro/SKILL.md)  
👉 **Interactive Live Mobile Showcase**: [`.agents/skills/mobile-uiux-pro/examples/mobile_showcase.html`](.agents/skills/mobile-uiux-pro/examples/mobile_showcase.html)

---

## 🖥️ 2. `desktop-uiux-pro` Highlights

### The 5 Laws of Desktop UI/UX:
1. **The 3-Tier Spatial Layout**: Collapsible sidebar navigation (64px/240px) + Top command bar (`⌘K`) + Asymmetric Bento grid work canvas.
2. **Proof Precedes Pitch**: Tech company logo clouds, live telemetry counters, and rating stars appear immediately below the hero headline. Abstract claims are backed by floating isometric live mockups.
3. **NeoSoftUI Aesthetics**: Layered obsidians (`#0B0F17`, `#101623`) + dual-layer glassmorphism (`backdrop-filter: blur(20px)`) + 10% high-impact Electric Indigo / Cyan accents.
4. **Keyboard & Precision Ergonomics**: Shortcuts (`⌘K`, `/`, `Shift + D`) embedded in tooltips; floating docked batch toolbar when 2+ table items are selected.
5. **Dense Enterprise Data Tables**: Sticky table headers, inline row filters, latency benchmarks, and optimistic UI updates.

👉 **View Full Desktop Skill**: [`.agents/skills/desktop-uiux-pro/SKILL.md`](.agents/skills/desktop-uiux-pro/SKILL.md)  
👉 **Interactive Live Desktop Showcase**: [`.agents/skills/desktop-uiux-pro/examples/desktop_showcase.html`](.agents/skills/desktop-uiux-pro/examples/desktop_showcase.html)

---

## 🚀 Example Prompts to Try with Your AI

### For Mobile Design:
```markdown
Using the mobile-uiux-pro skill, design a 4-step mindful reflection onboarding flow with interactive tags, a progress stepper, and a thumb-anchored CTA.
```

### For Desktop SaaS Design:
```markdown
Using the desktop-uiux-pro skill, architect a real-time analytics dashboard with an asymmetric Bento grid, ClickHouse latency counters, and a NeoSoftUI dark theme.
```

---

## 🔬 Empirical Data Foundation

These skills are not theoretical. They were synthesized by analyzing **over 950+ visual designs and real-world case studies** across:
- **@siren.uix**: Creator of the NeoSoftUI design system and Motvin asset platform.
- **@webdesignssphere**: Elite agency behind high-converting SaaS platforms and mindful mobile onboarding.
- **@webstarinfotech**: Specialists in luxury fashion eCommerce and high-contrast editorial typography.
- **@deluxewebsite**: Curators of modern interactive sliders, micro-interactions, and conversion patterns.

The automatic scraper used to collect and catalog the dataset is included in this repository: [`scrape_uiux_instagram.py`](scrape_uiux_instagram.py).

---

## 📂 Repository Structure

```
├── .agents/skills/
│   ├── mobile-uiux-pro/
│   │   ├── SKILL.md                          <- Universal Mobile AI Skill
│   │   └── examples/
│   │       └── mobile_showcase.html          <- Live Interactive Mobile Demo
│   └── desktop-uiux-pro/
│       ├── SKILL.md                          <- Universal Desktop AI Skill
│       └── examples/
│           └── desktop_showcase.html         <- Live Interactive Desktop Demo
├── ui_ux_references/                         <- 950+ Downloaded Curated UI/UX Screens
├── saas_analytics_neosoftui.html             <- Full Production SaaS Landing Page
├── scrape_uiux_instagram.py                  <- Reference Downloader & Cataloger
├── README.md                                 <- You Are Here
├── skills-lock.json                          <- Agent Skills Registry
└── LICENSE                                   <- MIT Open Source License
```

---

## 📄 License

This repository is distributed under the **MIT License**. Feel free to use, modify, share, and incorporate these skills into your own projects, agents, and design workflows.
