# 📚 AI Study Plan Generator Agent

An intelligent multi-agent AI system built with **CrewAI** and **Ollama (Llama 3)** that automatically generates personalized day-by-day study plans for any subject and exam timeline.

## 🎯 Project Overview

This project implements a **multi-agent AI workflow** where two specialized agents collaborate to produce a structured, realistic study plan based on a given subject and number of available days.

## 🤖 Agents

| Agent | Role |
|---|---|
| **Subject Analyst** | Breaks the subject into 6–10 key topics, ordered from foundational to advanced |
| **Study Planner** | Converts the topic list into a day-by-day study schedule with goals and tips |

## ⚙️ Tech Stack

- **Python 3.11**
- **CrewAI** — Multi-agent framework
- **Ollama** — Local LLM server
- **Llama 3** — Language model (runs locally, no API key needed)
- **LiteLLM** — LLM interface layer
- **Jupyter Notebook** — Development environment

## 🧪 Test Inputs

The notebook was tested on 3 different inputs:

- **Input 1:** Python Programming — 7 days
- **Input 2:** Machine Learning — 14 days
- **Input 3:** Data Structures and Algorithms — 10 days

## 🚀 How to Run

**Prerequisites:**
- Anaconda or Python 3.11+
- Ollama installed from [https://ollama.com/download](https://ollama.com/download)
- Llama 3 model downloaded

**Steps:**

```bash
# 1. Pull the Llama 3 model
ollama pull llama3

# 2. Start Ollama server
ollama serve

# 3. Install dependencies
pip install crewai crewai-tools langchain-ollama litellm python-dotenv

# 4. Open the notebook
jupyter notebook RollNo_Agent.ipynb

# 5. Run all cells from top to bottom
```

## 📁 Project Structure

```
├── RollNo_Agent.ipynb        # Main notebook
├── Agent Building - Ollama.ipynb  # Reference notebook (provided by instructor)
└── README.md
```

## 📝 Sample Output

```
Day 1 — Topic: Variables and Data Types
Goal: Understand basic data types in Python
Tip: Start by reviewing syntax before diving into advanced topics

Day 2 — Topic: Control Structures
Goal: Master if-else, for loops, while loops
Tip: Practice writing small code snippets daily
...
```

## 🔑 Key Concepts Demonstrated

- Multi-agent collaboration with sequential processing
- Local LLM integration (no internet or API cost)
- Dynamic inputs — same crew handles any subject and timeline
- Agent specialization — each agent has a focused role

## 👨‍🎓 Assignment Info

- **Course:** Artificial Intelligence
- **Assignment:** MID Part-B — AI Agent in Python
- **Tool:** CrewAI + Ollama (Llama 3)

