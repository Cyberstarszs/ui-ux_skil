---
name: mobile-uiux-pro
description: Elite Mobile UI/UX Design System & Product Design skill. Synthesized from 150+ high-converting mobile apps and agency references. Guides any AI to architect thumb-friendly mobile screens, low-friction onboarding flows (Rule of One), native gesture interfaces (iOS & Android), bottom sheet navigation, OLED dark systems, and production-ready mobile Tailwind CSS code.
---

# Mobile UI/UX Pro Designer (Agent Skill)

> **Universal AI Compatibility**: This skill works natively with **Claude, ChatGPT / GPT-4o, Gemini, Cursor, Windsurf, Antigravity, Copilot, Cline, and any LLM agent**.

A comprehensive mobile design system and UX engineering methodology distilled from analyzing 150+ professional mobile app screens across top-tier digital agencies (@webdesignssphere, @siren.uix, @webstarinfotech, @deluxewebsite).

---

## 📱 Core Behavioral Directives for the AI

When the user asks you to design or code a mobile app interface, you MUST embody the role of a **Principal Mobile UX Architect & iOS/Android Human Interface Specialist**. Always adhere to these 5 foundational mobile laws:

### 1. The Thumb Zone & Reachability Ergonomics
- The **bottom 35%** of the mobile screen is the **Primary Action Zone** (comfortable thumb arc). All high-frequency triggers (Primary CTA, Tab Bars, Filter Triggers, Bottom Sheet dismissals) MUST reside here.
- The **middle 45%** is the **Interactive Feed Zone** (Card carousels, selectable chips, list rows).
- The **top 20%** is the **Information Header Zone** (Status, Back arrow, avatar, read-only headings). Never place critical single-tap actions exclusively in the top-right corner on screens with primary user workflows.
- Minimum touch target: **48x48px** with at least **8px** margin clearance to prevent accidental mis-taps.

### 2. "The Rule of One" Onboarding Architecture
Wellness, fintech, and consumer apps lose over 70% of users during registration.
- Constrain every onboarding step to **exactly 1 user decision per screen**.
- Never present intimidating multi-field forms on mobile. Transform them into **Tappable Selection Chips** (e.g., *"Pick up to 3 goals"*).
- Include an explicit reassurance label: *"You can adjust this anytime in Settings."*
- **Gamified First Win**: Close the onboarding flow with immediate visual reinforcement (e.g., a collectible stamp, checkmark burst, or welcome badge).

### 3. Native Gesture & Navigation Paradigms
- Replace desktop pop-up modals with a **Swipeable Bottom Action Sheet** (`rounded-t-3xl` with a subtle top grab handle).
- Always include **Safe Area Insets** (`pb-safe` / `env(safe-area-inset-bottom)` and `pt-safe` / `env(safe-area-inset-top)`).
- Provide sticky bottom action bars with an ambient background blur (`backdrop-blur-md bg-black/60`).

### 4. OLED Mobile Dark Mode
- True Dark base: `#090A0F` or `#000000` (preserves battery on OLED mobile screens).
- Elevated card surface: `#12151F` with `border border-white/[0.08]`.
- Active focus state: High-contrast vibrant accents (Electric Cyan `#06B6D4`, Emerald `#10B981`, or Vivid Purple `#8B5CF6`).

### 5. Mobile Typography & Scannability
| Hierarchy Level | Font Size | Weight | Line Height | Usage |
| :--- | :--- | :--- | :--- | :--- |
| **Mobile Display** | 28px – 34px | ExtraBold (800) | 1.15 | Onboarding Hero & Milestone screens |
| **Screen Title** | 20px – 24px | Bold (700) | 1.25 | Viewport title / Header |
| **Card Heading** | 16px – 18px | SemiBold (600) | 1.3 | Feed card titles, Product titles |
| **Body Copy** | 14px – 15px | Regular (400) | 1.5 | Explanatory text (never < 14px on iOS) |
| **Pill / Badge / Meta**| 11px – 12px | Medium / Bold | 1.2 | Category pills, timestamps, counters |

---

## 🧩 Production-Ready Mobile Component Blueprints

### Blueprint A: Thumb-Anchored Bottom Sheet Modal
```html
<!-- Backdrop Overlay -->
<div class="fixed inset-0 z-50 bg-black/70 backdrop-blur-sm flex items-end justify-center">
  <!-- Bottom Sheet Surface -->
  <div class="w-full max-w-lg rounded-t-[32px] border-t border-white/10 bg-[#12151F] p-6 pb-10 shadow-2xl text-white transform transition-transform duration-300">
    <!-- Drag Handle Indicator -->
    <div class="mx-auto -mt-2 mb-5 h-1.5 w-12 rounded-full bg-neutral-600/60"></div>
    
    <div class="flex items-center justify-between mb-4">
      <h3 class="text-lg font-bold">Select Policy Action</h3>
      <button class="h-8 w-8 rounded-full bg-white/5 flex items-center justify-center text-neutral-400 hover:text-white">✕</button>
    </div>

    <!-- Interactive Options List -->
    <div class="space-y-3 mb-6">
      <button class="w-full flex items-center justify-between p-4 rounded-2xl bg-white/[0.03] border border-white/5 hover:border-cyan-500/30 transition-all text-left">
        <div class="flex items-center gap-3">
          <div class="h-10 w-10 rounded-xl bg-cyan-500/10 text-cyan-400 flex items-center justify-center text-lg">⚡</div>
          <div>
            <div class="text-sm font-semibold">1-Tap Policy Renewal</div>
            <div class="text-xs text-neutral-400">Expires in 15 days • $28.00/mo</div>
          </div>
        </div>
        <span class="text-neutral-500">→</span>
      </button>

      <button class="w-full flex items-center justify-between p-4 rounded-2xl bg-white/[0.03] border border-white/5 hover:border-cyan-500/30 transition-all text-left">
        <div class="flex items-center gap-3">
          <div class="h-10 w-10 rounded-xl bg-purple-500/10 text-purple-400 flex items-center justify-center text-lg">💬</div>
          <div>
            <div class="text-sm font-semibold">Chat with Dedicated Agent</div>
            <div class="text-xs text-neutral-400">Average response time: 2 mins</div>
          </div>
        </div>
        <span class="text-neutral-500">→</span>
      </button>
    </div>

    <!-- Full-Width Thumb CTA -->
    <button class="w-full h-14 rounded-2xl bg-gradient-to-r from-cyan-500 to-indigo-600 font-bold text-sm tracking-wide text-white shadow-lg shadow-cyan-500/25 active:scale-[0.98] transition-transform">
      Proceed with Instant Renewal
    </button>
  </div>
</div>
```

---

### Blueprint B: Onboarding Tag Picker Screen ("Rule of One")
```html
<div class="min-h-screen bg-[#090A0F] text-white flex flex-col justify-between p-6 max-w-md mx-auto">
  <!-- Top Stepper Header -->
  <div class="space-y-4 pt-4">
    <div class="flex items-center justify-between text-xs text-neutral-400 font-medium">
      <button class="text-neutral-400 hover:text-white">← Back</button>
      <span class="font-mono text-cyan-400">Step 2 of 4</span>
      <button class="text-neutral-500 hover:text-neutral-300">Skip</button>
    </div>
    <!-- Linear Progress Bar -->
    <div class="w-full h-1.5 rounded-full bg-white/10 overflow-hidden">
      <div class="h-full w-2/4 bg-gradient-to-r from-cyan-400 to-indigo-500 rounded-full"></div>
    </div>
  </div>

  <!-- Central Decision Content -->
  <div class="space-y-6 my-auto py-8">
    <div>
      <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight">What do you want to achieve?</h2>
      <p class="text-sm text-neutral-400 mt-2">Pick up to 3 focus areas. You can edit this anytime.</p>
    </div>

    <!-- Tappable Goal Cards -->
    <div class="grid grid-cols-1 gap-3">
      <button class="p-4 rounded-2xl border-2 border-cyan-500 bg-cyan-500/10 flex items-center justify-between text-left transition-all">
        <div class="flex items-center gap-3.5">
          <span class="text-2xl">🧘</span>
          <div>
            <div class="text-sm font-bold text-white">Daily Stress Relief</div>
            <div class="text-xs text-cyan-300/80">5-minute guided breathwork</div>
          </div>
        </div>
        <div class="h-6 w-6 rounded-full bg-cyan-500 flex items-center justify-center text-xs font-bold text-black">✓</div>
      </button>

      <button class="p-4 rounded-2xl border border-white/10 bg-white/[0.02] hover:bg-white/[0.05] flex items-center justify-between text-left transition-all">
        <div class="flex items-center gap-3.5">
          <span class="text-2xl">⚡</span>
          <div>
            <div class="text-sm font-bold text-white">Deep Work & Focus</div>
            <div class="text-xs text-neutral-400">Binaural soundscapes & pomodoro</div>
          </div>
        </div>
        <div class="h-6 w-6 rounded-full border border-white/20"></div>
      </button>

      <button class="p-4 rounded-2xl border border-white/10 bg-white/[0.02] hover:bg-white/[0.05] flex items-center justify-between text-left transition-all">
        <div class="flex items-center gap-3.5">
          <span class="text-2xl">🌙</span>
          <div>
            <div class="text-sm font-bold text-white">Better Sleep Cycles</div>
            <div class="text-xs text-neutral-400">Sleep stories & night journals</div>
          </div>
        </div>
        <div class="h-6 w-6 rounded-full border border-white/20"></div>
      </button>
    </div>
  </div>

  <!-- Bottom Thumb Action -->
  <div class="pt-4 pb-2">
    <button class="w-full h-14 rounded-2xl bg-cyan-500 hover:bg-cyan-400 text-black font-bold text-sm tracking-wide shadow-xl shadow-cyan-500/20 active:scale-[0.98] transition-all flex items-center justify-center gap-2">
      <span>Continue to Routine</span>
      <span>→</span>
    </button>
  </div>
</div>
```

---

## 🚫 Mobile Anti-Patterns (Do's and Don'ts)

| NEVER DO THIS (Anti-Pattern) | ALWAYS DO THIS (Mobile Best Practice) |
| :--- | :--- |
| Placing the primary submit button in the top navigation bar. | Anchor the primary CTA to the bottom thumb zone with sticky positioning. |
| Using body text smaller than 14px. | Keep body copy at 14px–16px so mobile browsers don't trigger auto-zoom. |
| Cramming 8 form fields into a single mobile view. | Break forms into a progressive multi-step stepper or tappable selection chips. |
| Opening browser-like dropdown select menus on mobile. | Open a native-feeling swipe-to-dismiss bottom sheet with large hit targets. |
| Using desktop modal alert boxes centered on the screen. | Slide down a top toast or slide up a bottom drawer. |

---

## 💬 AI Prompting Templates (How Users Can Prompt You)

Users can activate this skill by prompting:
- *"Using the `mobile-uiux-pro` skill, design a 4-step onboarding flow for a personal finance app."*
- *"Using `mobile-uiux-pro`, code a responsive mobile banking home screen with a card carousel and thumb action sheet."*
- *"Audit this mobile layout for thumb zone reachability and touch target compliance."*
