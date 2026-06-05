# Day 5 - Context Engineering

This is Day 5 of my 60-Day AI Challenge. Today I learned about context engineering and how giving more information to the AI changes the quality of the output.

What is Context Engineering?

Context engineering means giving the AI enough background before you ask it something. Instead of just asking a question directly, you tell it who you are, what you already know, what you want, and how you like to learn. That way the AI gives you something that fits your situation instead of a generic answer.

I used to think prompt engineering was just about wording things better. Today I understood that the real upgrade is giving better context, not just better words.

The Two Prompts

Prompt A had no context at all. I just typed: Create a 30-day learning roadmap.

Prompt B had full context. I added my situation as a B.Tech CS student, my existing skills in Python, Data Analysis, and Web Development, my goal to become an AI or ML engineer, 4 hours available per day, intermediate experience level, and a preference for hands-on project-based learning.

Output A - What I Got Without Context

Claude gave a standard 30-day ML roadmap. It was clean and well structured but it was clearly meant for anyone, not specifically for me.

The structure was:
* Week 1 - Foundations with NumPy, Pandas, EDA
* Week 2 - Supervised ML with Sklearn, XGBoost, Kaggle
* Week 3 - Deep Learning with PyTorch, BERT, W&B
* Week 4 - Deployment with FastAPI, Docker, Cloud

Total was 120 hours across 30 days with 4 portfolio projects and 1 live deployment.

Week 1 daily tasks were things like broadcasting and vectorisation, GroupBy and merge in Pandas, Matplotlib charts, hypothesis testing, and a final notebook on Titanic or House Prices dataset.

Resources given were Kaggle Learn, the Python for Data Analysis book by Wes McKinney, and the StatQuest YouTube channel.

Screenshots:

![Prompt A - Roadmap Overview](prompt_a_1.png)
![Prompt A - Week 1 Daily Tasks](prompt_a_2.png)
![Prompt A - Day 30 Outcomes](prompt_a_3.png)
![Prompt A - Paths After Day 30](prompt_a_4.png)

Output B - What I Got With Context

Claude gave a personalized roadmap with goal set to SWE and ML together, intermediate level, hands-on style, and 4 plus hours per day.

Week 1 milestone was DSA foundations solid and first portfolio project live.

Daily tasks were:
* Day 1-2: Arrays, strings, hashmaps and solve 10 LeetCode easy problems with 2 hours DSA and 2 hours project setup
* Day 3-4: Stacks, queues, sliding window and 10 more problems with 2 hours DSA and 2 hours practice
* Day 5-6: Binary search and two pointers and build a CLI task manager in Python with 1.5 hours DSA and 2.5 hours project
* Day 7: Review and push project to GitHub and write README with 4 hours on project and portfolio

Resources were NeetCode 150 list on LeetCode, NeetCode.io video walkthroughs, and Python standard library docs for collections and heapq.

First project was a CLI Task Manager, a command line app with add, delete, filter tasks, file persistence using JSON, and basic search.

Screenshots:

![Prompt B - Week 1 Personalized Roadmap](prompt_b_1.png)
![Prompt B - Week 1 Resources and Project](prompt_b_2.png)

Comparison

Prompt A gave a generic roadmap that anyone could use. Prompt B gave a roadmap that matched my actual skills and goals. The daily tasks in B had exact time splits. The first project in B used Python skills I already have. With Prompt A I would need to do extra planning before starting. With Prompt B I could start on Day 1 directly.

What I Observed

Which roadmap felt more personalized?

Prompt B was clearly more personalized. It knew I was aiming for SWE and ML together, that I already know Python, and that I prefer building things. Prompt A was good but it felt like something I could find on any blog.

Which roadmap would I actually follow?

Prompt B. The time splits are practical. The first project fits what I already know. I could open it on Day 1 and know exactly what to do. Prompt A was motivating to read but needed more planning before I could act on it.

What role did context play?

Context changed everything. Without context the AI assumed I was a beginner in ML with no coding skills and gave a standard path. With context it built something around my actual situation with my skills and my time.

The main thing I noticed is that the more specific the context, the more useful the output. It is not about writing a longer prompt. It is about giving the AI the right information.

Key Learnings

* Giving context is more important than changing the wording of a prompt
* Without context, AI gives a generic best-practice answer
* With context, AI gives something you can start using immediately
* Context engineering means treating the AI like a collaborator who needs to know your situation
* The quality of the output depends directly on the quality of information you provide
