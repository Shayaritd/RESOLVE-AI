# 🚀 AgentFlow AI

### Human-in-the-Loop Autonomous AI Workflow Platform

<p align="center">
  <b>Build reliable AI agents that can think, execute, pause, request approval, and continue with human guidance.</b>
</p>

<p align="center">
  LangGraph • FastAPI • Next.js • Python • LLM Agents • Human Approval Workflows
</p>

---

## 🌟 Overview

AgentFlow AI is a production-ready framework for building **controlled autonomous AI agents**.

Unlike traditional AI assistants that execute tasks without supervision, AgentFlow introduces **human-in-the-loop intelligence**, allowing users to review, approve, modify, or reject AI decisions before execution.

The platform enables:

* 🤖 Autonomous AI agents
* 🧠 Persistent memory across conversations
* ⏸️ Workflow interruption and resume
* ✅ Human approval checkpoints
* 🔄 Real-time streaming responses
* 🌐 Multi-provider LLM support

---

# ✨ Key Highlights

## 🧩 Human-Controlled AI Execution

AI workflows can pause at critical decision points:

```
User Request
      ↓
AI Planning
      ↓
Human Approval
      ↓
AI Execution
      ↓
Final Response
```

Users can:

✅ Approve AI actions
✏️ Modify generated outputs
❌ Reject and provide feedback
🔁 Resume execution from checkpoints

---

# 🏗️ System Architecture

```
                 User
                  |
                  ↓
        ┌─────────────────┐
        │  Next.js UI     │
        │ Chat Interface  │
        └─────────────────┘
                  |
                  ↓
        ┌─────────────────┐
        │ FastAPI Backend │
        └─────────────────┘
                  |
                  ↓
        ┌─────────────────┐
        │ LangGraph Agent │
        └─────────────────┘
                  |
        ┌─────────┴─────────┐
        ↓                   ↓
  LLM Provider        Memory Store
(OpenAI/Gemini/etc.)  Checkpoints
```

---

# 🚀 Features

## 🤖 Intelligent AI Agents

* Agent-based reasoning workflows
* Tool calling support
* Dynamic decision making
* Multi-step task execution

## ⏸️ Workflow Interruptions

Pause AI execution whenever human input is required.

Example:

```
AI:
"I created a report draft."

Human:
Approve / Edit / Reject

AI:
Continue execution...
```

---

## 🧠 Long-Term Memory

The system remembers:

* User preferences
* Previous conversations
* Workflow history
* Past decisions

---

## 🔄 Time Travel Debugging

Restore previous workflow states:

```
Checkpoint A
      ↓
Checkpoint B
      ↓
Checkpoint C

        ↘
       Fork New Path
```

Developers can test different AI decisions without losing previous executions.

---

# 🛠️ Tech Stack

## Backend

| Technology | Purpose                      |
| ---------- | ---------------------------- |
| Python     | Core programming language    |
| FastAPI    | API framework                |
| LangGraph  | Agent workflow orchestration |
| LangChain  | LLM integration              |
| SQLite     | Workflow persistence         |

## Frontend

| Technology | Purpose             |
| ---------- | ------------------- |
| Next.js    | Web application     |
| React      | UI components       |
| TypeScript | Type safety         |
| SSE        | Real-time streaming |

## AI Models Supported

* OpenAI
* Google Gemini
* Anthropic Claude
* Groq
* Mistral
* Ollama

---

# 📂 Project Structure

```
AgentFlow-AI/

│
├── backend/
│   ├── main.py
│   ├── agent.py
│   ├── graph.py
│   ├── memory.py
│   ├── tools.py
│   └── requirements.txt
│
├── frontend/
│   ├── app/
│   ├── components/
│   └── package.json
│
├── docker-compose.yml
├── Dockerfile
└── README.md
```

---

# ⚡ Installation

## Clone Repository

```bash
git clone <repository-url>

cd AgentFlow-AI
```

---

## Backend Setup

```bash
cd backend

python -m venv .venv

pip install -r requirements.txt

python main.py
```

Backend:

```
http://localhost:8000
```

---

## Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Frontend:

```
http://localhost:3000
```

---

# 🔌 API Endpoints

| Endpoint   | Description                    |
| ---------- | ------------------------------ |
| `/start`   | Start AI workflow              |
| `/resume`  | Continue interrupted workflow  |
| `/stream`  | Stream AI response             |
| `/history` | View checkpoints               |
| `/fork`    | Create alternate workflow path |
| `/health`  | System status                  |

---

# 🎯 Real-World Applications

### 🏢 Enterprise AI Assistants

Automate business processes while keeping humans in control.

### 📄 Document Review

AI drafts → Human verifies → AI publishes.

### 💬 Customer Support

AI handles requests and escalates complex cases.

### 📊 Research Automation

AI collects information and generates reports.

---

# 🧪 Testing

Run tests:

```bash
pytest -v
```

---

# 🐳 Docker Support

Run the complete application:

```bash
docker compose up --build
```

---

# 📈 Future Improvements

* Multi-agent collaboration
* Role-based permissions
* Vector database memory
* Voice-based AI assistant
* Cloud deployment support

---

# 👨‍💻 Developer

Built with:

❤️ Python
⚡ LangGraph
🚀 FastAPI
🎨 Next.js

---

⭐ If you find this project useful, consider starring the repository.
