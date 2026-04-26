# 🌸 PetalLogic AI
## 🧠 AI-Powered DSA Learning & Visualization Platform

PetalLogic AI is a next-generation learning system that helps users **understand Data Structures & Algorithms through AI-generated explanations, interactive chat, and flowchart-based visualization**.

Instead of memorizing algorithms, users can:
- 💬 Ask AI doubts in natural language
- 📊 Visualize step-by-step execution using flowcharts
- 🧠 Learn through structured AI explanations
- 📈 Track learning progress dynamically

---

# 🚀 Why PetalLogic AI?

Traditional learning is:
❌ Static  
❌ Hard to visualize  
❌ Memorization-heavy  

PetalLogic AI makes it:
✔ Interactive  
✔ Visual  
✔ AI-driven  
✔ Concept-focused  

---

# 🏗 System Overview

- 🧩 Microservices backend (Spring Boot + Eureka + Gateway)
- 💬 AI Chat Engine (Ollama Qwen3 local LLM)
- 🌐 React-based interactive frontend
- 📊 Flowchart visualization engine (React Flow)
- 🗄 MySQL database for persistence

---

# 🌿 Core Idea

> “Every algorithm is like a blooming structure — PetalLogic AI helps you see how it grows step by step.”

---

# ⚙️ Tech Stack

- Spring Boot 3+
- Spring Cloud Gateway + Eureka
- React 18
- Tailwind CSS
- MySQL
- Ollama Qwen3
- React Flow

---

# 🧠 Key Features

- AI-powered DSA tutor
- Step-by-step flowchart generation
- Chat-based learning interface
- Topic-wise structured learning system
- Progress tracking dashboard
- Microservices architecture

---

# 🌸 Vision

To transform algorithm learning from **text-based memorization → visual AI-driven understanding**.

---

* 🧰 Prerequisites (software + setup)
* 🧠 LLM architecture (Ollama Qwen)
* 🏗 Microservices design
* 🗄 Database schema (real tables)
* 🌐 React architecture
* 🔌 API gateway flow
* ⚙️ End-to-end system data flow

---

# 🏗 PetalLogic AI — SYSTEM DESIGN DOCUMENT

````md id="petallogic_system_design"
# 🏗 PetalLogic AI — System Design

## 🌸 Overview

PetalLogic AI is an AI-powered DSA learning system that combines:
- Microservices architecture (Spring Boot)
- Local LLM reasoning (Ollama Qwen3)
- Interactive React frontend
- Flowchart-based visualization engine
- Structured learning + progress tracking

---

# ⚙️ 1. PREREQUISITES (DEVELOPMENT SETUP)

## 🧰 Required Software

### 🖥 Backend
- Java 17+
- Spring Boot 3+
- Maven / Gradle
- MySQL 8+
- IntelliJ IDEA

### 🌐 Frontend
- Node.js 18+
- React 18+
- Vite
- Tailwind CSS
- VS Code

### 🧠 AI Layer
- Ollama installed locally
- Qwen3 model (recommended)
```bash
ollama run qwen:7b
````

### 🔧 Dev Tools

* Postman (API testing)
* Docker (optional for microservices)
* Git + GitHub
* Redis (optional caching)

---

# 🧠 2. AI / LLM ARCHITECTURE

## 💬 Ollama Qwen3 Flow

User Query → Chat Service → Prompt Engine → Ollama Qwen3 → Structured Response → Frontend Renderer

---

## 🧩 AI Output Structure

All AI responses MUST follow this format:

```json
{
  "explanation": "step-by-step reasoning",
  "code": "optional code snippet",
  "flowchart": {
    "nodes": [],
    "edges": []
  },
  "complexity": "O(n)"
}
```

---

## 🧠 Prompt Engineering Layer

We enforce:

* structured JSON output
* step-by-step reasoning
* algorithm decomposition

---

# 🏗 3. MICROSERVICES ARCHITECTURE

## 🔥 Core Services

### 1. Auth Service

* JWT login/register
* user authentication

### 2. User Service

* profile management
* progress tracking

### 3. Topic Service

* DSA topics (arrays, trees, DP)
* content management

### 4. Chat AI Service

* connects to Ollama Qwen3
* processes prompts
* returns structured AI response

---

## 🌐 API Gateway (Spring Cloud Gateway)

* Single entry point
* Routes requests to microservices
* Handles authentication filtering

---

## 🔍 Service Discovery

* Netflix Eureka Server
* Registers all microservices
* Enables dynamic scaling

---

# 🗄 4. DATABASE DESIGN (MYSQL)

---

## 👤 users

```sql
id (PK)
name
email
password
created_at
```

---

## 📚 topics

```sql
id (PK)
title
category
difficulty
description
```

---

## 📈 user_progress

```sql
id (PK)
user_id (FK)
topic_id (FK)
progress_percentage
last_accessed
```

---

## 💬 chat_history

```sql
id (PK)
user_id (FK)
query
response_json
timestamp
```

---

## 🌳 flowcharts

```sql
id (PK)
topic_id (FK)
nodes_json
edges_json
created_at
```

---

# 🌐 5. REACT FRONTEND ARCHITECTURE

## 📁 Folder Structure

```
src/
 ├── components/
 ├── pages/
 ├── services/
 ├── hooks/
 ├── context/
 ├── utils/
```

---

## 🧩 Core Pages

* Login / Register
* Dashboard
* Topic Explorer
* AI Chat Interface
* Flowchart Viewer

---

## 💬 AI Chat UI Flow

User Input → API Call → Chat Service → Ollama → Response → Render UI + Flowchart

---

# 🔌 6. API FLOW ARCHITECTURE

## Example Flow

### User asks:

> "Explain Binary Search"

### System flow:

1. React → Gateway
2. Gateway → Chat Service
3. Chat Service → Prompt Engine
4. Prompt → Ollama Qwen3
5. Response → JSON structured output
6. Frontend renders:

   * explanation
   * code
   * flowchart

---

# 🧠 7. FLOWCHART ENGINE

## Tech

* React Flow

## Structure

```json
{
  "nodes": [
    { "id": "1", "data": "Start" },
    { "id": "2", "data": "Check mid" }
  ],
  "edges": [
    { "from": "1", "to": "2" }
  ]
}
```

---

# ⚡ 8. SYSTEM GOALS

✔ AI-driven learning
✔ Visual understanding of DSA
✔ Structured explanations
✔ Real-time interaction
✔ Scalable microservices

---

# 🌸 9. CORE PRINCIPLE

> “Understanding algorithms is not memorization — it is visualization of logic flow.”

---

```

---

# 🚀 WHAT YOU NOW HAVE

You now have:

✔ Professional GitHub README (your project)  
✔ Full system design document  
✔ AI architecture (Ollama Qwen3 flow)  
✔ Microservices breakdown  
✔ Database schema  
✔ React architecture  
✔ API flow design  
✔ Flowchart system design  

---

# 🔥 NEXT BEST STEP (HIGHLY RECOMMENDED)

If you want to go serious production-level next, I can build:

### ⚙️ 1. ACTUAL SPRING BOOT MICROSERVICE SCAFFOLD
- Eureka server
- API gateway
- Auth service
- Chat AI service

### ⚛️ 2. REACT UI STARTER KIT
- login page
- dashboard
- chat UI
- flowchart UI

### 🧠 3. OLLAMA QWEN PROMPT ENGINE CODE
- structured response generator
- JSON enforcement system

### 🧪 4. POSTMAN TEST COLLECTION + TEST STRATEGY
- full system testing plan

Just say 👍
```
