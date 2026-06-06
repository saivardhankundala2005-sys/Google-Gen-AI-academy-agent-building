# Google-Gen-AI-academy-agent-building
A collection of projects, exercises, and agents built as part of the Google Gen AI Academy course, focusing on LLM workflows and autonomous agents.
# Google Gen AI Academy: Agent Building 🤖

Welcome to the **Google Gen AI Academy Agent Building** repository. This project is a comprehensive, hands-on guide to constructing autonomous, intelligent AI agents using the **Google Agent Development Kit (ADK)** and the Gemini 2.5 ecosystem. 

This repository tracks my journey through learning how to give LLM-powered agents superpowers: connecting them to custom tools, engineering multi-agent orchestration systems, and managing robust conversational states.

---

## 🚀 Key Learning Objectives & Core Pillars

The implementations inside this repository focus on four fundamental capabilities of modern AI engineering:

1. **Building Foundational Agents:** Designing simple, single-purpose agents from scratch using specified instructions and base models.
2. **Custom Tool Integration (Function Tools):** Extending an agent's capabilities by bridging it to real-world, live external APIs.
3. **Multi-Agent Orchestration (Agent-as-a-Tool):** Crafting a hierarchical system where a primary coordinator agent delegates specialized tasks to sub-agents.
4. **Conversational Memory Management:** Implementing session states so agents can retain context, process sequential user feedback, and carry out complex multi-turn planning.

---

## 📦 Project Architecture & Walkthrough

The project is structured sequentially across the following core exercises:

### 🔑 Part 0: Setup & Authentication
Configuring the workspace using the new Google Gen AI SDK (`google-genai` and `google-adk`). It handles secure authentication via Google Colab (`auth.authenticate_user()`) and initializes the project environment globally inside Vertex AI:
```python
import google.adk as adk
from google.adk.agents import Agent
from google.adk.runners import Runner
from google.adk.sessions import InMemorySessionService
