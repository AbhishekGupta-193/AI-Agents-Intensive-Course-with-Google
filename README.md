#  5-Day AI Agents Intensive Course with Google

This repository documents my learnings, assignments, and hands-on implementations from **Google’s 5-Day AI Agents Intensive Course**, designed by Google’s ML researchers and engineers.  
The program explores the foundations and practical applications of AI agents — from design principles to deployment-ready systems.

---

## 📚 Course Overview

The 5-Day Intensive Course provides a structured learning path to understand how intelligent agents operate and interact within real-world ecosystems.  
It focuses on five key components of agent systems:

- **Models** – The intelligence layer powering reasoning and decisions  
- **Tools** – Extending agent capabilities through APIs and integrations  
- **Orchestration** – Coordinating multi-agent workflows and collaboration  
- **Memory** – Preserving context for continuity and learning  
- **Evaluation** – Measuring agent reliability, accuracy, and adaptability  

By the end of this program, agents transition from prototype-level LLMs to **production-ready autonomous systems** with strong governance, interoperability, and observability.

---

## 🗓️ Daily Progress

### **Day 1 – Introduction to Agents**

**Focus:**  
Understanding the concept of AI agents, their taxonomy and capabilities, and the need for **Agent Operations (Agent Ops)** — a discipline focused on ensuring reliability, governance, and security through well-defined identities and constrained policies.

**Day 1 Work:**
  - **Build your first AI Agent** – Created an agent capable of using Google Search to fetch and respond with up-to-date information  
  - **Build your first Multi-Agent System** – Developed a team of specialized agents and explored different communication and orchestration patterns  

**Learning Summary:**  
Acquired a foundational understanding of AI agents as autonomous, goal-oriented systems that can reason, act, and collaborate effectively.  
Gained practical exposure to agent creation using ADK and learned the basics of multi-agent system coordination and architecture.

---

### Day 2 – Agent Tools & Model Context Protocol (MCP)

**Focus:**  
Day 2 focuses on extending agent capabilities using **tools** and enabling interoperability through the **Model Context Protocol (MCP)**. You also work with long-running operations and learn best practices for designing reliable and safe tools.


**Agent Tools – Key Concepts**
- Tools enable agents to **take actions or access data beyond their training**.
- Well-designed tools should be:
  - **Safe** – validate all inputs  
  - **Deterministic** – predictable, consistent outputs  
  - **Idempotent** – safe to retry  
  - **Purpose-specific** – minimal and clear functionality  

**Model Context Protocol (MCP)**
MCP provides a standardized way for agents, tools, and external systems to communicate.

**MCP Architecture**
- **Server** – exposes tools or resources  
- **Client** – agent consuming tools  
- **Transport Layer** – JSON-RPC / WebSockets  

**Why MCP Matters**
- Ensures **interoperability** across tools and agent frameworks  
- Scales well for **enterprise environments**  
- Establishes a consistent interaction model for multi-agent systems  

---

### Day 3 – Context Engineering: Sessions & Memory

**Focus**
Day 3 dives into **context engineering**, focusing on how agents manage information across turns (Sessions) and across conversations (Memory). You learn how to build stateful, coherent, and personalized agents using ADK.

**Context Engineering**
- Dynamically assembling relevant information for the LLM.
- Using **context compaction** to fit essential details within the context window.
- Enables personalized, multi-turn interactions.

**Sessions**
- Represents the **active conversation container**.
- Stores:
  - User messages  
  - Agent responses  
  - Events and intermediate reasoning  
- Enables coherent multi-turn conversations.

**Memory**
- Long-term persistence beyond a single session.
- Allows agents to recall:
  - User preferences  
  - Previous tasks  
  - Historical interactions  


**Core Learnings**
- **Context Engineering** fundamentals  
- Maintaining conversation history using **Sessions & Events**  
- Using **Persistent Storage** for long-term recall  
- Managing **Session State** via structured fields  
- Understanding manual state handling (pros/cons)  
- Preparing for real-world production constraints  

---

### Day 4 – Agent Quality & Evaluation Framework

**Focus**
Day 4 focuses on ensuring **quality, reliability, and transparency** in AI agents. It introduces a complete evaluation framework built on observability and scalable assessment methods such as LLM-as-a-Judge and Human-in-the-Loop (HITL) evaluation.

**Observability: The Foundation of Agent Quality**
Observability enables deep insight into how and why an agent makes decisions. It relies on three key pillars:

**Logs — *“The Diary”***
- Records detailed event-by-event activity  
- Captures prompts, tool calls, errors, and agent reasoning steps  
- Essential for debugging and auditing  

**Traces — *“The Narrative”***
- Connects logs into a sequential workflow  
- Shows relationships between actions  
- Helps visualize the end-to-end decision-making pipeline  

### 🔹 **Metrics — *“The Health Report”***
- Tracks quantitative signals such as:
  - Latency  
  - Error rates  
  - Tool success/failure  
  - Token usage  
- Useful for monitoring agent performance over time  

**Evaluation Frameworks**

**LLM-as-a-Judge**
- Uses a large language model to **score or critique** agent responses  
- Enables high-scale, automated evaluation  
- Useful for measuring:
  - Accuracy  
  - Relevance  
  - Safety  
  - Tool usage quality  

**Human-in-the-Loop (HITL)**
- Human reviewers evaluate complex or high-stakes outputs  
- Complements automated scoring methods  
- Ideal for:
  - Edge cases  
  - Safety-sensitive scenarios  
  - Quality assurance before deployment  

---


