# Day 5: Context Engineering — Prompt A vs Prompt B

Hey everyone! Welcome to **Day 5** of my 60-Day AI Challenge. Today I explored **Context Engineering** — one of the most powerful concepts in working with AI systems. The key experiment: running the *same task* with and without context and observing how drastically the output changes.

---

## 🧠 What is Context Engineering?

**Context Engineering** is the practice of designing and structuring the information you give to an AI model — not just *what* you ask, but *who you are*, *what you already know*, *what you need*, and *how you prefer to learn*.

It's a step above prompt engineering. Instead of just tweaking the wording of a question, you curate the **entire input environment** — background, constraints, goals, skill level, time available — so the AI acts as a true strategic partner rather than a generic search engine.

> **Key insight:** The quality of AI output is directly proportional to the quality of context you provide.

---

## 🧪 The Experiment: Prompt A vs Prompt B

### 📝 Prompt A (No Context — Generic)

```
Create a 30-day learning roadmap.
```

### 📝 Prompt B (With Context — Personalized)

```
Create a 30-day learning roadmap.

Context:
- Current Situation: Student (B.Tech Computer Science)
- Current Skills: Python, Data Analysis, Web Development
- Goal: Become an AI/ML Engineer
- Available Time: 4 hours per day
- Experience Level: Intermediate
- Preferred Learning Style: Projects (Hands-on)

Include:
- Weekly milestones
- Daily tasks
- Resources
- Projects
- Final outcome

Make it practical and beginner-friendly.
```

---

## 📊 Output A — Generic Roadmap (No Context)

**Title:** Your 30-day ML roadmap
**Tagline:** Intermediate · 4 hrs/day · Project-driven · Production-ready outcome

| Stat | Value |
|------|-------|
| Duration | 30 Days |
| Total Practice | 120 hrs |
| Portfolio Projects | 4 |
| Live Deployments | 1 |

### Weekly Structure

| Week | Theme | Tools |
|------|-------|-------|
| Week 1 | Foundations | NumPy · Pandas · EDA |
| Week 2 | Supervised ML | Sklearn · XGBoost · Kaggle |
| Week 3 | Deep Learning | PyTorch · BERT · W&B |
| Week 4 | Deployment | FastAPI · Docker · Cloud |

### Week 1 Milestone
> Master NumPy, Pandas, and Matplotlib. Complete a full EDA on a real-world dataset with statistical insights.

### Week 1 Daily Tasks
1. Broadcasting, vectorisation, linear algebra toolkit from scratch
2. GroupBy, multi-index, merge/join, apply() on a messy CSV
3. Matplotlib + seaborn: heatmaps, pair plots, distributions
4. Hypothesis testing, CLT, correlation vs causation
5. Encoding, scaling, imputation, skewness correction
6–7. Full notebook on Titanic / House Prices — 15+ charts + written insights

### Resources
- **Kaggle Learn** — Pandas & Data Cleaning (Free · Interactive · ~4 hrs)
- **Python for Data Analysis** — Wes McKinney (Chapters 4–10 · NumPy + Pandas bible)
- **StatQuest** — Statistics playlist (YouTube · Free · Visual-first explanations)

### Project 1 of 4: Exploratory Data Analysis Report
> Pick any Kaggle dataset with 10k+ rows. Produce a polished Jupyter notebook: 15+ visualisations, data quality audit, and 5 written insights.
>
> **Tags:** NumPy · Pandas · Seaborn · Statistical thinking · Jupyter

### What You'll Have on Day 30
- ✅ 4 GitHub projects (one with a live public URL)
- ✅ Full ML stack (Data → model → API → cloud)
- ✅ Kaggle ranking (Top 30% competition submission)
- ✅ Core tools mastered (Sklearn, XGBoost, PyTorch, HuggingFace)
- ✅ Transformer model (Fine-tuned BERT on custom data)
- ✅ Job-ready portfolio (Ready for ML engineer applications)

### Paths After Day 30
`Computer vision (YOLO, Detectron2)` `LLM fine-tuning (GPT-style)` `MLOps at scale (Kubeflow)` `Kaggle Expert rank` `Open-source contributions`

### Screenshot — Prompt A Output
![Prompt A Output - Generic ML Roadmap Overview](prompt_a_1.png)
![Prompt A Output - Week 1 Daily Tasks](prompt_a_2.png)
![Prompt A Output - Day 30 Outcomes](prompt_a_3.png)
![Prompt A Output - Paths After Day 30](prompt_a_4.png)

---

## 📊 Output B — Personalized Roadmap (With Context)

**Title:** 30-day Personalized Learning Roadmap
**Conversation:** 60 Days of AI project in Claude

| Parameter | Value |
|-----------|-------|
| Goal | SWE + ML/DS |
| Level | Intermediate |
| Style | Hands-on |
| Daily Hours | 4+ |

### Week 1 Milestone
> **DSA foundations solid + first portfolio project live**

### Week 1 Daily Tasks

| Days | Task | Time Split |
|------|------|-----------|
| 1–2 | Arrays, strings, hashmaps — solve 10 LeetCode easy problems | 2h DSA + 2h project setup |
| 3–4 | Stacks, queues, sliding window — 10 more problems + patterns | 2h DSA + 2h practice |
| 5–6 | Binary search + two pointers — build a CLI task manager in Python | 1.5h DSA + 2.5h project |
| 7 | Review + push project to GitHub + write README | 4h project + portfolio |

### Resources
- **LeetCode** — NeetCode 150 list (free)
- **NeetCode.io** — video walkthroughs per pattern
- **Python Docs** — standard library (collections, heapq)

### Week 1 Project: CLI Task Manager
> Build a command-line app with add/delete/filter tasks, file persistence (JSON), and basic search.
> Keeps Python + file I/O sharp while being portfolio-worthy.
>
> **Tag:** SWE

### Screenshot — Prompt B Output
![Prompt B Output - Personalized Roadmap Week 1 Milestone](prompt_b_1.png)
![Prompt B Output - Week 1 Resources and Project](prompt_b_2.png)

---

## 🔍 Comparison: Prompt A vs Prompt B

| Feature | Prompt A (No Context) | Prompt B (With Context) |
|---|---|---|
| **Personalization** | ❌ Generic ML path for anyone | ✅ Tailored to CS student with Python/Web skills |
| **Goal alignment** | Generic ML engineer path | SWE + ML/DS dual-track |
| **Daily tasks** | Broad topics (EDA, NumPy) | Specific (10 LeetCode problems, exact time splits) |
| **Time splits** | Not specified per task | 2h DSA + 2h project (precise) |
| **Resources** | General (Kaggle, StatQuest) | Targeted (NeetCode 150, pattern-based learning) |
| **First project** | EDA report (data science focus) | CLI Task Manager (practical + portfolio-ready) |
| **Style match** | Assumed project-driven | Explicitly hands-on / project-based |
| **Actionability** | High-level roadmap | Day-by-day actionable plan |
| **Relevance** | 70% relevant to my profile | 95%+ relevant to my profile |

---

## 💡 Key Learnings

### 1. Which Roadmap Feels More Personalized?
**Prompt B (with context) is dramatically more personalized.** It knows I'm aiming for SWE + ML/DS, that I'm intermediate level, that I prefer hands-on learning, and that I have 4+ hours daily. The daily tasks reflect *my* existing Python knowledge and skip the absolute beginner steps. Prompt A gave a solid roadmap, but it could have been written for anyone on the internet.

### 2. Which Roadmap Would I Actually Follow?
**Prompt B — without question.** The time splits (2h DSA + 2h project) are realistic and specific. The first project (CLI Task Manager) builds directly on skills I already have. NeetCode 150 is a well-known, community-validated resource. I can start Day 1 immediately without needing to figure out "what exactly do I do first?"

Prompt A, while impressive, requires me to do more planning work myself — "120 hours across 30 days" is motivating, but it's not as immediately actionable.

### 3. What Role Did Context Play in Improving the Result?

Context transformed the AI from a **textbook** into a **personal coach**:

| Without Context | With Context |
|---|---|
| Generic best practices | Specific to my skill gaps |
| One-size-fits-all structure | Adapted to my 4h/day schedule |
| Assumed learning style | Matched my hands-on preference |
| Broad resource list | Curated resources (NeetCode 150 for patterns) |
| Standard ML track | Dual SWE + ML/DS track |

> **The biggest lesson:** Context engineering isn't about writing longer prompts — it's about giving the AI the *right* information so it can make intelligent decisions on your behalf.

### 4. The Engineering Mindset Shift
Before today, I thought good prompting meant using better words or clearer instructions. After today, I understand that **context is the raw material** that the AI uses to personalize everything. Just like a doctor can't diagnose without your medical history, Claude can't give you a personalized plan without your background, goals, and constraints.

**Context Engineering = Treating the AI like a smart collaborator, not a search engine.**

---

## 🎯 Takeaways

- ✅ **Always provide context** — skill level, time, goals, and learning style make a massive difference
- ✅ **Specificity compounds** — the more specific your context, the more actionable the output
- ✅ **Context engineering > prompt engineering** for complex, personalized tasks
- ✅ **Roadmaps without context are generic** — they might be accurate but not *yours*
- ✅ **The AI is only as smart as the context you give it**

---

This is Day 5 done! The shift from prompt engineering to context engineering is a fundamental upgrade in how I'll use AI tools going forward. 🚀
