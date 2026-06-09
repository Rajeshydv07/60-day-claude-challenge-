# Day 9 — Building NutriScope with Claude AI 🥗

## Overview
On Day 9 of the 60-day Claude challenge, I used Claude AI to generate a full-featured **NutriScope** nutrition tracking web application in two iterations — an MVP version and an enhanced version — then compared the results.

---

## What is NutriScope?
NutriScope is a **Precision Nutrition Tracker** — a single-file HTML application that lets users:
- Set up a personal profile (age, weight, height, activity level, dietary preference, goals)
- Log daily food intake from a built-in food database
- Visualize macros (calories, protein, carbs, fat) and micronutrients
- Get smart AI-generated recommendations
- Track deficiencies and excesses
- View interactive charts (energy ring, macro donut, radar chart, bar chart)

---

## Files in this folder

| File | Description |
|---|---|
| `NutriScope_MVP.html` | Version 1 — MVP generated with Prompt 1 |
| `NutriScope_Enhanced.html` | Version 2 — Enhanced app generated with Prompt 2 |
| `day9.md` | This documentation file |

---

## Prompt 1 — MVP Version
**Goal:** Generate a basic but functional nutrition tracker with:
- Profile setup form
- Food log table
- Macro tracking dashboard
- Basic charts

**Result:** `NutriScope_MVP.html` — 1,894 lines, ~87 KB  
Dark-themed app with 6 navigation sections: Dashboard, Profile, Food Log, Meal Planner, Risk, and Learn.

---

## Prompt 2 — Enhanced Version
**Goal:** Enhance the MVP with improved UI, better charts, and cleaner layout.

**Result:** `NutriScope_Enhanced.html` — 1,530 lines, ~58 KB  
Refined app with 5 sections: Dashboard, Profile, Food Log, Nutrients, and Recommendations.

---

## Comparison: MVP vs Enhanced

| Feature | MVP (`NutriScope_MVP.html`) | Enhanced (`NutriScope_Enhanced.html`) |
|---|---|---|
| **Lines of Code** | ~1,894 | ~1,530 |
| **File Size** | ~87 KB | ~58 KB |
| **Navigation** | 6 tabs (Dashboard, Profile, Log, Plan, Risk, Learn) | 5 tabs (Dashboard, Profile, Log, Nutrients, Recs) |
| **Typography** | Inter + DM Mono | Inter + Space Grotesk |
| **Logo Icon** | 🥗 | 🔬 |
| **Header Layout** | Logo + Nav in header | Logo + separate nav bar |
| **Energy Display** | Bar chart (Chart.js) | Animated ring/donut with % overlay |
| **Macro Chart** | Donut + bar charts | Cleaner donut chart |
| **Stat Cards** | Gradient accent glow | Top-border accent line (--card-accent) |
| **Recommendations** | Alert-box style | rec-card style with icon |
| **Toast Notifications** | ❌ No | ✅ Yes (slide-up toast) |
| **BMI/BMR Display** | Targets preview card | Full Body Composition Snapshot |
| **Meal Planner** | ✅ Yes (7-day grid) | ❌ Removed |
| **Risk Section** | ✅ Yes | ❌ Removed |
| **CSV Upload** | ✅ Yes | ❌ Removed |
| **Mobile Nav** | ✅ Bottom mobile nav | ❌ Responsive tabs instead |
| **Card Hover** | ❌ None | ✅ Border color transition |
| **Scrollbar** | Custom (6px) | Custom (6px, rounded) |
| **Responsiveness** | ✅ 640px / 900px breakpoints | ✅ 768px / 480px breakpoints |

---

## Key Learnings

1. **Claude generates complete apps in one shot** — Both HTML files are fully self-contained with embedded CSS and JavaScript. No external dependencies except Chart.js CDN.

2. **Iteration refines code** — The enhanced version is more concise (~27% fewer lines) while maintaining feature parity. Claude naturally tightened the CSS, simplified the layout, and improved typography choices in the second pass.

3. **Design philosophy shifted** — MVP focused on information density (6 sections, more features). Enhanced version focused on UX quality (fewer sections, better visual hierarchy, toast feedback, energy ring).

4. **Prompting strategy matters** — A clearer, more specific second prompt produced code that was smaller and better structured. The MVP had legacy patterns (inline styles everywhere), while the enhanced version used more semantic CSS variables.

5. **Single-file HTML apps are powerful** — Both apps run 100% offline without any backend, server, or framework. Just open in a browser.

6. **AI-first development workflow** — Using Claude as the primary code generator, then comparing iterations, is a valid modern development workflow for rapid prototyping.

---

## Tools Used
- **Claude AI** (claude.ai) — Code generation
- **Chart.js 4.4.1** — Data visualizations
- **Google Fonts** — Inter, DM Mono, Space Grotesk
- **HTML/CSS/JS** — Single-file app, no framework

---

## How to Run
1. Open `NutriScope_MVP.html` or `NutriScope_Enhanced.html` in any browser
2. Go to **Profile** tab and fill in your details
3. Click **Save Profile & Calculate Targets**
4. Go to **Food Log** and start adding meals
5. Return to **Dashboard** to see your nutrition data

> ⚠️ **Disclaimer:** NutriScope is for educational purposes only. Nutritional data is approximate. Always consult a registered dietitian for personalized medical advice.

---

## Commit Info
- **Day:** 9 / 60
- **Date:** June 9, 2026
- **Challenge:** 60-Day Claude AI Challenge
- **Topic:** AI-Assisted Web App Development — NutriScope Nutrition Tracker
