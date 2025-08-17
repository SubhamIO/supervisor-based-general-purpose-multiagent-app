# 🧠 Agentic AI Application — Multi-Agent Supervisor System

A full-stack, modular, agentic AI system powered by LangGraph, LangChain, and multiple external tools. Built to handle intelligent task decomposition, multi-step reasoning, and user-friendly interaction.

---


## 🧩 Architecture Overview

```
                      ┌────────────┐
                      │ Supervisor │
                      └─────┬──────┘
                            ↓
        ┌──────────┬──────────────┬─────────────┬───────────────┐
        ↓          ↓              ↓             ↓               ↓
    Greeting    Enhancer       Coder     Maths Reasoner     Researcher
        │          │              │             │               │
        └──────────┴────┬─────────┴─────────────┴───────────────┘
                        ↓
                 Tool Execution Layer
            (Python REPL, Tavily, PubMed, etc.)
```

---


## 🛠️ Tech Stack

| Layer              | Tools/Frameworks                          |
| ------------------ | ----------------------------------------- |
| **Agents & Logic** | `LangChain`, `LangGraph`                  |


---


## 🧠 Agents & Tools

### 👷 Supervisor Agent

- Central brain of the system
    
- Delegates tasks to other agents
    
- Makes decisions based on outputs and history
    

### ✨ Enhancer Agent

- Improves clarity, tone, and relevance of intermediate results
    

### 💬 Greeting Agent

- Handles user onboarding and initial context setting
    

### 🧑‍💻 Coder Agent

- Writes and debugs code
    
- Uses `PythonREPL` for live execution
    

### 🧠 Maths Reasoner

- Handles symbolic & numerical problems
    
- Uses `calculator` and `PythonREPL`
    

### 🔍 Researcher

- Finds factual data and references using:
    
    - `Tavily`
        
    - `DuckDuckGo`
        
    - `Wikipedia`
        
    - `PubMed`

---


## 💡 Features

✅ Real-time **streaming chatbot interface**  
✅ **Multi-session / Multi-chat** support  
✅ Modular **agent-tool orchestration**  
✅ **Dynamic memory** per chat  




## 🧪 Tooling Integration

|Tool|Purpose|
|---|---|
|**Tavily**|Fast multi-source web search|
|**Wikipedia**|Structured encyclopedic info|
|**DuckDuckGo**|Lightweight search fallback|
|**PubMed**|Scientific paper lookup|
|**PythonREPL**|Code execution sandbox|
|**Calculator**|Basic arithmetic + formulas|
