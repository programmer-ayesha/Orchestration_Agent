# Orchestration_Agent

# 🧠 Language Orchestration with Agentic AI (OpenAI Agents SDK)

This project demonstrates how to build a modular and professional **Language Orchestrator Agent** using the `openai-agents` Python SDK. It detects the input language and dynamically selects the appropriate translator agent (Spanish or French) using tool handoffs.

---

## 🚀 What It Does

- 🔍 **Detects the input language** using a `Detect Language Agent`
- 🧠 **Orchestrates translation flow** using the `Orchestrator Agent`
- 🌐 **Translates** user message using either:
  - 🇪🇸 `Spanish Agent`
  - 🇫🇷 `French Agent`

All agents use the **LiteLLM wrapper** to connect to models like Gemini (`gemini/gemini-2.0-flash`).

---

## 🧩 Agents Overview

| Agent Name         | Purpose                                      |
|--------------------|----------------------------------------------|
| `Detect Language Agent` | Detects the language of input text            |
| `Spanish Agent`         | Translates any input to Spanish             |
| `French Agent`          | Translates any input to French              |
| `Orchestrator Agent`    | Orchestrates the flow using the other tools |

---

## 📦 How to Run

1. Clone the repo or open the notebook in Colab
2. Install dependencies:
   ```bash
   pip install openai-agents
