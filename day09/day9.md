# Day 9 — Building NutriScope with Claude AI 🔬

## Overview
On Day 9 of the 60-day Claude challenge, I used Claude AI to generate a full-featured **NutriScope** — a Precision Nutrition Tracker — as a single self-contained HTML application.

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

| File | Description |
|---|---|
| `NutriScope.html` | Full NutriScope app — Precision Nutrition Tracker |
| `day9.md` | This documentation file |

---

## App Features

### 📊 Dashboard
- 4 stat cards: Calories, Protein, Carbs, Fat
- Animated **energy ring** showing % of daily goal consumed
- **Macro Split** donut chart (Chart.js)
- Top Deficiencies & Top Excesses progress bars
- Macro Progress tracker

### 👤 Profile
- Input: Age, Gender, Height, Weight
- Activity level selector (Sedentary → Extremely Active)
- Dietary preference (Vegetarian / Non-Veg / Eggetarian)
- Goal selector (Maintain / Lose / Gain weight)
- Auto-calculates **BMI**, **BMR** (Mifflin-St Jeor), and **TDEE**

### ➕ Food Log
- Select from built-in food database
- Enter quantity + unit (grams, ml, piece, cup, tbsp)
- Running totals: Calories, Protein, Carbs, Fat, Fiber
- Remove individual entries or clear all

### 🧪 Nutrients
- Full micronutrient breakdown table
- Status indicators (Adequate / Low / Excess)

### 💡 Recommendations
- Smart recommendation cards based on deficiencies and goals

---

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Structure & semantics |
| Vanilla CSS | Styling with CSS variables, dark theme |
| Vanilla JavaScript | All logic, calculations, state |
| Chart.js 4.4.1 (CDN) | Energy ring + macro donut charts |
| Google Fonts: Inter + Space Grotesk | Typography |

---

## Design Highlights
- 🌑 **Dark theme** — base color `#0a0b0f`
- 🎨 **Accent palette** — Purple `#6c63ff`, Teal `#00d4aa`, Coral `#ff6b6b`, Amber `#ffd166`, Cyan `#06b6d4`
- ✨ **Animated energy ring** with glow effect
- 🔔 **Toast notifications** for save confirmations
- 📱 **Fully responsive** — adapts to mobile (768px / 480px breakpoints)
- 🃏 **Card hover effects** with border color transitions

---

## How to Run
1. Open `NutriScope.html` in any browser
2. Go to **Profile** tab → fill in your details → click **Save Profile & Update Targets**
3. Go to **Food Log** → select food → add entries
4. Return to **Dashboard** to see your nutrition data update live
5. Check **Nutrients** and **Recommendations** tabs for insights

> ⚠️ **Disclaimer:** NutriScope is for educational purposes only. Nutritional data is approximate. Always consult a registered dietitian for personalized medical advice.

---

## Key Learnings

1. **Claude generates complete, production-quality apps** — The app is 100% self-contained (~58 KB, 1,530 lines) with no build step required.
2. **Single-file HTML is powerful** — Works fully offline, no server needed, just open in a browser.
3. **AI-assisted design** — Claude chose a professional dark theme, typography, and layout without being asked for specific designs.
4. **Chart.js integration** — Claude correctly integrated Chart.js via CDN and wired it to dynamic JS data.
5. **CSS variables** — The design system uses CSS custom properties extensively, making the theme fully maintainable.

---

## Commit Info
- **Day:** 9 / 60
- **Date:** June 9, 2026
- **Challenge:** 60-Day Claude AI Challenge
- **Topic:** AI-Assisted Web App Development — NutriScope Precision Nutrition Tracker
