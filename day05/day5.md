# Day 5 - Context Engineering

This is Day 5 of my 60-Day AI Challenge. Today I learned about context engineering and how giving more information to the AI changes the quality of the output.

---

## What is Context Engineering?

Context engineering basically means giving the AI enough background before you ask it something. Instead of just asking a question directly, you tell it who you are, what you already know, what you want, and how you like to learn. That way the AI can give you something that actually fits your situation instead of a generic answer.

I used to think prompt engineering was just about wording things better. Today I understood that the real upgrade is giving better context, not just better words.

---

## The Two Prompts

### Prompt A - No Context

```
Create a 30-day learning roadmap.
```

### Prompt B - With Context

```
Create a 30-day learning roadmap.

Context:
- Current Situation: Student (B.Tech Computer Science)
- Current Skills: Python, Data Analysis, Web Development
- Goal: Become an AI/ML Engineer
- Available Time: 4 hours per day
- Experience Level: Intermediate
- Preferred Learning Style: Projects

Include:
- Weekly milestones
- Daily tasks
- Resources
- Projects
- Final outcome

Make it practical and beginner-friendly.
```

---

## Output A - What I Got Without Context

Claude gave a standard 30-day ML roadmap. It looked clean and well-structured but it was clearly meant for anyone, not specifically for me.

Overview:
- 30 Days, 120 total hours, 4 portfolio projects, 1 live deployment
- Week 1: Foundations - NumPy, Pandas, EDA
- Week 2: Supervised ML - Sklearn, XGBoost, Kaggle
- Week 3: Deep Learning - PyTorch, BERT, W&B
- Week 4: Deployment - FastAPI, Docker, Cloud

Week 1 milestone was to master NumPy, Pandas, and Matplotlib and complete a full EDA on a real-world dataset.

Daily tasks for Week 1:
- Day 1: Broadcasting, vectorisation, linear algebra from scratch
- Day 2: GroupBy, merge/join, apply() on a messy CSV
- Day 3: Matplotlib and seaborn charts
- Day 4: Hypothesis testing, CLT, correlation vs causation
- Day 5: Encoding, scaling, imputation
- Day 6-7: Full notebook on Titanic or House Prices

Resources given:
- Kaggle Learn - Pandas and Data Cleaning
- Python for Data Analysis by Wes McKinney
- StatQuest Statistics playlist on YouTube

By Day 30, the roadmap said I would have 4 GitHub projects, a full ML stack from data to cloud, a Kaggle ranking in top 30%, and a job-ready portfolio.

**Screenshots:**

![Prompt A - Roadmap Overview](prompt_a_1.png)
![Prompt A - Week 1 Daily Tasks](prompt_a_2.png)
![Prompt A - Day 30 Outcomes](prompt_a_3.png)
![Prompt A - Paths After Day 30](prompt_a_4.png)

---

## Output B - What I Got With Context

Claude gave a roadmap called "30-day personalized learning roadmap" and the parameters it picked up were:
- Goal: SWE + ML/DS
- Level: Intermediate
- Style: Hands-on
- Daily hours: 4+

Week 1 milestone: DSA foundations solid and first portfolio project live.

Week 1 daily tasks:
- Day 1-2: Arrays, strings, hashmaps - solve 10 LeetCode easy problems (2 hours DSA + 2 hours project setup)
- Day 3-4: Stacks, queues, sliding window - 10 more problems plus patterns (2 hours DSA + 2 hours practice)
- Day 5-6: Binary search and two pointers - build a CLI task manager in Python (1.5 hours DSA + 2.5 hours project)
- Day 7: Review and push project to GitHub, write README (4 hours project and portfolio)

Resources:
- LeetCode - NeetCode 150 list (free)
- NeetCode.io - video walkthroughs per pattern
- Python Docs - standard library like collections and heapq

First project: CLI Task Manager - a command-line app with add, delete, filter tasks, file persistence using JSON, and basic search.

**Screenshots:**

![Prompt B - Week 1 Personalized Roadmap](prompt_b_1.png)
![Prompt B - Week 1 Resources and Project](prompt_b_2.png)

---

## Comparison

| | Prompt A | Prompt B |
|---|---|---|
| Personalization | Generic, for anyone | Specific to my skills and background |
| Daily tasks | Broad topics | Exact tasks with time splits |
| First project | EDA report | CLI Task Manager |
| Resources | General (Kaggle, StatQuest) | Targeted (NeetCode 150) |
| Could I start immediately | Needed more planning | Yes, from Day 1 |

---

## What I Observed

**Which roadmap felt more personalized?**

Prompt B was clearly more personalized. It knew I was aiming for SWE and ML together, that I already know Python, and that I prefer building things. The daily tasks were specific enough that I could start without figuring out the details myself. Prompt A was good but it felt like a roadmap I could find on any blog.

**Which roadmap would I actually follow?**

Prompt B. The time splits like 2 hours DSA and 2 hours project are practical. The first project uses Python skills I already have. I could open it on Day 1 and know exactly what to do.

Prompt A was motivating to read but I would need to do extra planning before starting.

**What role did context play?**

Context made the difference between a generic plan and a plan that fits me. Without context, the AI assumed things - it assumed I was a beginner in ML, that I only wanted an ML path, that I had no existing coding skills. With context, it built something around my actual situation.

The biggest thing I noticed is that the more specific the context, the more useful the output. It is not about writing a longer prompt. It is about giving the AI the right information so it can make smart decisions.

---

## Key Learnings

- Giving context is more important than changing the words of a prompt
- Without context, AI gives you a generic best-practice answer
- With context, AI gives you something you can actually use from Day 1
- Context engineering is basically treating the AI like a collaborator who needs to know your situation before helping
- The quality of output depends directly on the quality of input you provide
