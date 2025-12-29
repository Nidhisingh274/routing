# 🤖 Agentic Content Router

An intelligent agentic workflow built with **LangGraph**, **LangChain**, and **Groq's LLaMA model** that automatically detects user intent and routes prompts to generate the correct output — a **story**, **joke**, or **poem** — without manual intervention.

---

## ✨ Features
- 🔀 **Automated Routing:** Uses an LLM-powered classifier to understand the user's request and pick the right node.
- 🧠 **Agentic Logic Flow:** Built with `StateGraph` to enable branching and controlled execution.
- ⚡ **Powered by Groq:** Ultra-fast inference using `llama-3.1-8b-instant`.
- 📌 **Modular Nodes:** Each node handles a specific task (story, joke, poem).
- 📈 **Visual Graph:** Generates a Mermaid graph for workflow visualization.

---

## 🛠️ Tech Stack
| Component | Description |
|-----------|--------------|
| **Groq API** | Fast LLM inference |
| **LangChain + LangGraph** | Workflow orchestration & routing |
| **Python** | Core implementation |
| **TypedDict + Pydantic** | Structured state & validation |

---

## 🚀 How It Works
1. The user enters a prompt.
2. Router model classifies the request into: `story`, `joke`, or `poem`.
3. Workflow moves to the respective LLM node.
4. Output is returned with context logging.

---
```bash
pip install langchain-groq langgraph python-dotenv
