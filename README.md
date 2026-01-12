# AI-Agent-Planning

This repository contains a project focused on **AI Agent Planning**, demonstrating how intelligent agents can reason about goals and generate structured action plans using classical planning techniques, assisted by a Large Language Model.

The project uses **Google Gemini** as the underlying AI model for agent reasoning and plan generation, combined with symbolic planning representations.

---

## 📌 Project Overview

Planning is a core capability of intelligent agents. Instead of reacting to a single prompt, a planning agent reasons about:
- The current state of the world
- Available actions and constraints
- A desired goal state

Using this information, the agent produces a **sequence of actions (a plan)** that leads from the initial state to the goal.

In this project, the reasoning and decision-making process is supported by the **Gemini model**, while the planning problems themselves are represented declaratively using PDDL.

---

## 🧠 Model Used

- **LLM:** Google Gemini  
- **Role of the model:**
  - Interpreting planning problems
  - Reasoning about goals and constraints
  - Assisting in plan generation and analysis

The Gemini model is used as an intelligent agent capable of understanding structured planning tasks and guiding the planning process.

---

### Files Description

- **AgenticAI.ipynb**  
  A Jupyter notebook that demonstrates agentic AI and planning concepts, including reasoning about goals and plans.

- **community_garden.pddl**  
  The planning *domain* definition, describing:
  - Actions
  - Preconditions
  - Effects
  - Objects and predicates

- **community_garden_problem_vX.pddl**  
  Multiple planning *problem instances* that define different initial states and goals for the same domain.

---

### Planning Concept

The planning setup follows the classical AI planning model:
- **Domain**: What actions exist and how they change the world
- **Problem**: Initial state + goal state
- **Planner**: Computes a valid action sequence that satisfies the goal

This approach allows testing different scenarios by changing only the problem file while keeping the domain fixed.

---

## ▶️ How to Run

### Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/shaysmer/AI-agent-palnning.git
   cd AI-agent-palnning

