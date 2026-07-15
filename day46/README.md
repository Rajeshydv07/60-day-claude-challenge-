# 🧠 Autonomous Agent Studio

An interactive multi-agent AI workflow that simulates how autonomous agents collaborate to create, evaluate, improve, and finalize high-quality long-form articles through an iterative feedback loop.

---

## 🚀 Overview

**Autonomous Agent Studio** demonstrates a complete AI agent orchestration system where multiple specialized agents work together to continuously improve content quality.

Instead of generating content in a single step, the application follows an iterative workflow:

```
Planner
   ↓
Executor
   ↓
Evaluator
   ↓
Critic
   ↓
Improver
   ↓
Memory Manager
   ↺ (Loop)
   ↓
Final Reviewer
```

The loop continues until a quality threshold, plateau detection, or iteration limit is reached.

---

## ✨ Features

- 📝 AI-powered article generation
- 🤖 Seven specialized autonomous agents
- 🔄 Continuous improvement feedback loop
- 📊 Real-time quality scoring
- 📈 Iteration history tracking
- 🧠 Memory Manager for context preservation
- 📋 Live activity log
- 🎯 Configurable quality threshold
- 🔁 Automatic stopping conditions
- ✅ Final QA review before publishing
- 📱 Responsive modern dashboard
- 🌙 Dark newsroom-inspired interface

---

## 🤖 Agent Responsibilities

### Planner
Creates a structured outline including sections, article angle, and required evidence.

### Executor
Generates the first complete article draft from the outline.

### Evaluator
Scores the draft based on:

- Clarity
- Depth
- Accuracy
- Engagement

Produces a composite quality score out of 100.

### Critic
Identifies the highest-impact improvements and provides actionable feedback.

### Improver
Rewrites the article using evaluator scores and critic suggestions.

### Memory Manager
Records improvements made during each iteration and preserves important context for future rounds.

### Final Reviewer
Performs the final proofreading, quality assurance, and publication-ready review.

---

## 🔄 Workflow

1. User enters topic and audience.
2. Planner creates the article structure.
3. Executor writes the initial draft.
4. Evaluator scores the content.
5. Critic generates improvement suggestions.
6. Improver revises the draft.
7. Memory Manager records progress.
8. Steps 4–7 repeat until stopping conditions are met.
9. Final Reviewer publishes the polished article.

---

## 🛑 Stopping Conditions

The iteration loop stops when any of the following occurs:

- Quality threshold achieved
- Score improvement plateaus
- Maximum iteration limit reached

---

## 📊 Dashboard Includes

- Live workflow visualization
- Active agent indicator
- Current draft preview
- Composite quality score
- Activity log
- Memory updates
- Iteration history
- Final performance summary

---

## 🛠️ Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript
- SVG Workflow Visualization
- Anthropic Claude API
- Responsive UI Design

---

## 📂 Project Structure

```
Autonomous-Agent-Studio/
│
├── index.html
├── README.md
└── assets/
```

---

## 💡 Future Enhancements

- Web search integration
- Fact-checking agent
- Citation generation
- Parallel draft comparison
- Human approval checkpoints
- Multi-format content generation
- Export to PDF and Markdown
- Additional evaluation metrics

---

## 🎯 Learning Outcomes

This project demonstrates:

- Multi-agent AI systems
- Agent orchestration
- Iterative AI workflows
- Autonomous decision-making
- Prompt engineering
- State management
- AI evaluation pipelines
- Human-inspired editorial processes

---

## 📸 Preview

The interface includes:

- Assignment setup panel
- Workflow visualization
- Draft editor
- Activity log
- Memory tracker
- Iteration history
- Performance dashboard
- Final publication summary

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository, improve the workflow, and submit pull requests.

---

## 📜 License

This project is intended for educational and research purposes.

---

### ⭐ If you found this project useful, consider giving it a star on GitHub!
