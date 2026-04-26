# 🌸 PetalLogic AI

## 🧠 Production-Grade AI-Powered DSA Learning & Visualization Platform

👨‍💻 Pavan Kalyan  
👩‍💻 Kruthika  
🤝 Co-Built Full Stack AI System (Microservices + LLM + Visualization)

---

# 🚀 Overview

**PetalLogic AI** is a production-grade intelligent learning platform that transforms Data Structures & Algorithms into:

- 🧠 AI-generated step-by-step explanations  
- 📊 Interactive flowchart visualizations  
- 💬 Conversational AI learning assistant  
- 📚 Structured topic-based learning system  
- ⚡ Real-time AI reasoning using local LLM (Ollama Qwen3)

---

# 🧠 Core Idea

> “Turn every algorithm into a visual, interactive, AI-explained learning experience.”

Instead of memorizing DSA:
✔ You interact with AI  
✔ You visualize execution  
✔ You understand logic step-by-step  

---

# 🏗️ System Architecture (Production Design)

```

```
                ┌──────────────────────┐
                │     React Frontend   │
                │ Dashboard + Chat UI  │
                └─────────┬────────────┘
                          │ REST / WebSocket
                          ▼
            ┌─────────────────────────────┐
            │ Spring Cloud API Gateway   │
            └────────────┬────────────────┘
                         │
 ┌───────────────────────┼────────────────────────┐
 ▼                       ▼                        ▼
```

┌──────────────┐   ┌────────────────┐   ┌────────────────────┐
│ Auth Service │   │ Topic Service  │   │ AI Orchestrator     │
│ JWT Security │   │ DSA Content    │   │ Prompt Engine       │
└──────────────┘   └────────────────┘   └─────────┬──────────┘
▼
┌──────────────────────┐
│ Ollama Qwen3 LLM     │
│ Local AI Engine      │
└─────────┬────────────┘
▼
┌──────────────────────┐
│ Flow Generator       │
│ (Graph JSON Engine)  │
└──────────────────────┘

```

---

# ⚙️ Microservices Architecture

## 1. 🔐 Auth Service
- JWT authentication
- User registration/login
- Role-based access

## 2. 📚 Topic Service
- DSA topics management
- problem catalog
- learning structure

## 3. 🤖 AI Orchestrator Service
- Prompt construction
- AI response structuring
- Ollama communication layer

## 4. 📊 Visualization Service
- Flowchart JSON generator
- Step-by-step execution mapping
- Graph builder engine

## 5. 🌐 API Gateway (Spring Cloud)
- Central routing layer
- Load balancing
- Request filtering

---

# 🤖 AI Pipeline

```

User Query
↓
Prompt Builder (Spring Boot)
↓
Ollama Qwen3 Model
↓
Structured JSON Output
↓
Flow Generator Service
↓
React UI Renderer

```

---

# 🧱 Tech Stack

## Backend
- Java 17+
- Spring Boot 3+
- Spring Cloud Gateway
- Eureka Server
- Spring Security (JWT)

## AI Layer
- Ollama (Qwen3 LLM)
- Prompt Engineering Engine
- JSON structured AI outputs

## Frontend
- React 18+
- React Flow (visualization)
- Axios (API calls)
- Tailwind CSS

## Database
- MySQL
- Redis (future caching layer)

---

# 🗄️ Database Design

## 👤 User Table
- id
- name
- email
- password
- role

## 📚 Topic Table
- id
- name
- difficulty
- description

## 🧠 AI History Table
- id
- user_id
- prompt
- response_json
- timestamp

## 📊 Progress Table
- id
- user_id
- topic_id
- completion_status

---

# 🌟 Key Features

## 🧠 AI Learning Engine
- Ask any DSA question
- Get structured AI explanation
- Step-by-step reasoning

## 📊 Flowchart Visualization
- Algorithm execution visualization
- Node-based step breakdown
- Interactive learning flow

## 💬 AI Chat System
- Chat-based learning interface
- Context-aware responses
- History tracking

## 📚 Topic System
- Structured DSA roadmap
- Difficulty-based learning
- Progress tracking

## 📈 Dashboard
- Learning analytics
- Progress tracking
- AI interaction history

---

# 🔁 Execution Model (Daily Build System)

👨‍💻 Pavan + 👩‍💻 Kruthika

Each day:
- 🧠 Learn system design + AI concepts
- 🛠 Build backend + frontend together
- 🔗 Integrate AI + UI + APIs
- 🧪 Test full feature increment

---

# 📅 Development Phases

## Phase 1 — Core Infrastructure
- Microservices setup
- API Gateway
- Eureka Server

## Phase 2 — Authentication System
- JWT security
- Login/register UI

## Phase 3 — Topic Engine
- DSA structure system
- API + UI integration

## Phase 4 — AI Engine
- Ollama integration
- Prompt engineering system

## Phase 5 — Visualization Engine
- Flowchart generator
- React Flow integration

## Phase 6 — Full System Integration
- AI + UI + backend sync
- End-to-end flow

## Phase 7 — Production Hardening
- performance tuning
- error handling
- deployment prep

---

# 🎯 Final Outcome

✔ AI-powered DSA tutor  
✔ Microservices backend system  
✔ React-based intelligent UI  
✔ Local LLM integration (Ollama Qwen3)  
✔ Flowchart-based learning engine  
✔ Production-ready architecture  

---

# ⚡ Vision

> “Make DSA learning as intuitive as watching a live system execution.”

---

# 🚀 Status

> 🟢 Active Development (30-Day Build Sprint)

---

# 🤝 Contributors (Shared Engineering Model)

👨‍💻 Pavan Kalyan — Full Stack + AI + System Design + Integration  
👩‍💻 Kruthika — Full Stack + AI + System Design + Integration  

## ⚠️ STRICT RULE

Both contributors will actively work across:

- 🧠 Backend (Spring Boot Microservices)
- 🌐 Frontend (React + UI/UX)
- 🤖 AI Layer (Ollama + Prompt Engineering)
- 🔌 Integration (API + End-to-End Flow)
- 🧱 System Design (Architecture + Data Flow)
- 🧪 Testing & Debugging

---

## 🔁 WORKING PRINCIPLE

> “No fixed roles. Only shared ownership of the entire system.”

Every feature must be:
- Designed together
- Built together (pair execution)
- Debugged together
- Integrated together

---

## 🎯 EXPECTED OUTCOME

Both contributors will:
✔ Understand full system architecture  
✔ Write backend and frontend code  
✔ Build AI integration logic  
✔ Handle system design decisions  
✔ Debug full-stack issues independently  

---

---
