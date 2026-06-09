# Day 9 — Building NutriScope with Claude AI 🔬

## Overview
On Day 9 of the 60-day Claude challenge, I used Claude AI to generate a full-featured **NutriScope** — a Precision Nutrition Tracker — in two iterations. First an MVP version, then an enhanced version. Both are single-file HTML apps with zero dependencies beyond Chart.js CDN.

---

## What is NutriScope?
NutriScope is a **Precision Nutrition Tracker** — a single-file HTML application that lets users:
- Set up a personal profile (age, weight, height, activity level, dietary preference, goals)
- Log daily food intake from a built-in food database
- Visualize macros (calories, protein, carbs, fat) via interactive charts
- Track deficiencies and excesses in real time
- Get personalized recommendations based on intake vs targets
- View BMI, BMR, and TDEE body composition snapshot

---

## Files in this folder

| File | Size | Description |
|---|---|---|
| `NutriScope_MVP.html` | ~87 KB · 1,894 lines | Version 1 — MVP generated with Prompt 1 |
| `NutriScope_Enhanced.html` | ~58 KB · 1,530 lines | Version 2 — Enhanced app generated with Prompt 2 |
| `day9.md` | — | This documentation file |

---

## MVP vs Enhanced — Comparison

| Feature | MVP (`NutriScope_MVP.html`) | Enhanced (`NutriScope_Enhanced.html`) |
|---|---|---|
| **Lines of Code** | ~1,894 | ~1,530 |
| **File Size** | ~87 KB | ~58 KB |
| **Navigation** | 6 tabs (Dashboard, Profile, Log, Plan, Risk, Learn) | 5 tabs (Dashboard, Profile, Log, Nutrients, Recs) |
| **Typography** | Inter + DM Mono | Inter + Space Grotesk |
| **Logo Icon** | 🥗 | 🔬 |
| **Header** | Logo + Nav in single header | Separate header + nav bar |
| **Energy Display** | Bar chart (Chart.js) | Animated ring/donut with % overlay |
| **Stat Cards** | Gradient accent glow | Top-border accent line (`--card-accent`) |
| **Recommendations** | Alert-box style | `rec-card` style with icon + description |
| **Toast Notifications** | ❌ No | ✅ Yes (slide-up toast) |
| **BMI/BMR Display** | Targets preview card | Full Body Composition Snapshot |
| **Meal Planner** | ✅ 7-day grid | ❌ Removed |
| **Risk Section** | ✅ Yes | ❌ Removed |
| **CSV Upload** | ✅ Yes | ❌ Removed |
| **Mobile Nav** | ✅ Bottom mobile nav | ❌ Responsive tabs instead |
| **Card Hover** | ❌ None | ✅ Border color transition |

---

## Enhanced Version — Feature Details

### 📊 Dashboard
- 4 stat cards: Calories, Protein, Carbs, Fat (with top color accent bar)
- Animated **energy ring** showing % of daily goal consumed
- **Macro Split** donut chart (Chart.js)
- Top Deficiencies & Top Excesses with progress bars
- Macro Progress tracker (Protein, Carbs, Fat, Fiber)

### 👤 Profile
- Input: Age, Gender, Height, Weight
- Activity level selector (Sedentary → Extremely Active)
- Dietary preference (Vegetarian / Non-Veg / Eggetarian)
- Goal selector (Maintain / Lose / Gain weight)
- Auto-calculates **BMI**, **BMR** (Mifflin-St Jeor), **TDEE**

### ➕ Food Log
- Select from 20 built-in Indian food items
- Enter quantity + unit (grams, ml, piece, cup, tbsp)
- Running totals row: Calories, Protein, Carbs, Fat
- Remove individual entries or clear all
- Toast notifications on actions

### 🧪 Nutrients
- Full micronutrient breakdown table (Iron, Calcium, Vit C, Vit D, Vit B12)
- Status badges: Very Low / Low / On Track / Excess
- Micronutrient coverage progress bars

### 💡 Recommendations
- Smart recommendation cards based on deficiencies and goals
- Icon + title + description layout

---

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Structure & semantics |
| Vanilla CSS | Styling with CSS variables, dark theme |
| Vanilla JavaScript | All logic, calculations, state management |
| Chart.js 4.4.1 (CDN) | Energy ring + macro donut charts |
| Google Fonts: Inter + Space Grotesk | Typography |
| localStorage | Persist profile + food log across sessions |

---

## Design Highlights
- 🌑 **Dark theme** — base color `#0a0b0f`
- 🎨 **Accent palette** — Purple `#6c63ff`, Teal `#00d4aa`, Coral `#ff6b6b`, Amber `#ffd166`, Cyan `#06b6d4`
- ✨ **Animated energy ring** with glow drop-shadow effect
- 🔔 **Toast notifications** for save confirmations (slide-up animation)
- 📱 **Fully responsive** — adapts to mobile (768px / 480px breakpoints)
- 🃏 **Card hover effects** with border color transitions

---

## How to Run
1. Open `NutriScope_MVP.html` or `NutriScope_Enhanced.html` in any browser
2. Go to **Profile** tab → fill in your details → click **Save Profile & Update Targets**
3. Go to **Food Log** → select food → add entries
4. Return to **Dashboard** to see your nutrition data update live
5. Check **Nutrients** and **Recommendations** tabs for insights

> ⚠️ **Disclaimer:** NutriScope is for educational purposes only. Nutritional data is approximate. Always consult a registered dietitian for personalized medical advice.

---

## Key Learnings

1. **Claude generates complete, production-quality apps** — Both files are 100% self-contained with no build step required.
2. **Iteration refines code** — Enhanced version is ~27% smaller (58 KB vs 87 KB) while being more polished.
3. **Single-file HTML is powerful** — Works fully offline, no server needed, just open in a browser.
4. **Design improves with iteration** — Second prompt produced cleaner typography, better visual hierarchy, and added toast feedback.
5. **CSS variables** — The design system uses CSS custom properties extensively, making the theme consistent and maintainable.
6. **localStorage** — Both apps persist user profile and food log across browser sessions without any backend.

---

## Commit Info
- **Day:** 9 / 60
- **Date:** June 9, 2026
- **Challenge:** 60-Day Claude AI Challenge
- **Topic:** AI-Assisted Web App Development — NutriScope Precision Nutrition Tracker (MVP + Enhanced)
