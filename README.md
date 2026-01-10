# 🧠 Agentic AI Projects

A curated collection of **Agentic AI systems** focused on reasoning, workflows, memory, and control.

These projects demonstrate how modern AI agents are designed **beyond basic LLM calls**, with emphasis on **routing, evaluation, memory, safety, and system orchestration**.

---

## 👀 Who This Repository Is For
- Recruiters evaluating **Agentic AI / AI Systems** skills  
- AI engineers exploring **LangGraph-based agent workflows**  
- Developers interested in **memory, caching, and controlled AI systems**

---

## 📌 Projects

### 01️⃣ Autonomous Research Agent
A research-grade **Retrieval-Augmented Generation (RAG)** agent for answering complex queries using documents.

**Key Highlights**
- PDF ingestion and intelligent chunking
- Vector embeddings with hybrid retrieval (Semantic + MMR)
- Query intelligence: expansion, decomposition, and HyDE
- Structured research-style responses
- Self-evaluation and retry logic using LangGraph

**Design Decisions**
- Hybrid retrieval balances relevance and diversity  
- Query intelligence improves recall and context quality  
- Self-evaluation ensures higher answer quality  

**Limitations & Future Work**
- Hallucination checks can be strengthened with grounding metrics  
- Cost and token tracking not yet implemented  

---

### 02️⃣ Multi Route Workflow
A **multi-agent workflow system** that routes user queries to the correct agent based on intent.

**Key Highlights**
- LLM-based routing with strict structured outputs
- Travel planning, RAG, and calculator agents
- Human-in-the-loop approval and modification
- LangGraph-based conditional workflows
- Execution step tracking for observability

**Design Decisions**
- Structured routing prevents uncontrolled agent behavior  
- Human-in-the-loop ensures safety and correctness  
- LangGraph enables clear, inspectable control flow  

**Limitations & Future Work**
- External APIs (booking, payments) are mocked  
- Workflow currently notebook-based  

---

### 03️⃣ Agentic AI with Memory, Tools & Cache
A production-oriented conversational agent with **long-term memory, caching, and safety controls**.

**Key Highlights**
- Persistent fact memory using SQLite
- Semantic cache using FAISS with LRU eviction
- Confidence-gated response storage
- Latency-aware execution (memory → cache → LLM)
- Hallucination reduction via fact-only answering

**Design Decisions**
- Memory-first strategy reduces latency and cost  
- Confidence gating prevents unsafe caching  
- Semantic cache improves repeat query performance  

**Limitations & Future Work**
- Fact schema is currently fixed  
- Memory expiration strategy can be added  

---

## 🛠 Tech Stack
**Python · LangChain · LangGraph · OpenAI / Ollama · FAISS · ChromaDB · SQLite · Jupyter Notebook**

---

## 📂 Repository Structure

```
agentic-ai-projects/
├── 01 Autonomous Research Agent/
│   └── agent.ipynb
├── 02 Multi Route Workflow/
│   └── agent.ipynb
└── 03 Agentic AI with Memory, Tools & Cache/
    └── agent.ipynb
```

---

## ⚠️ Notes
- Each project is fully implemented in a **single notebook** to preserve reasoning flow.
- Environment variables are excluded for security.
- Use `.env.example` to configure required keys.

---

## 👤 Author

**Hemant**  
**Agentic AI / AI Systems Engineer**

Focused on building:
- Reliable and controllable AI agents  
- Memory-driven and cost-aware systems  
- Human-in-the-loop workflows  
- Safe and production-oriented AI architectures  

---

> *Less prompting. More engineering.*
