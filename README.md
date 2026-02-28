# Fraud Investigation AI Workbench Suite 🔍

Welcome to the **Fraud AI Workbench** repository. This project showcases a series of AI-powered solutions for fraud detection, ranging from basic analytics dashboads to advanced multi-agent systems and graph-based reasoning.

## 🚀 Overview

This repository contains four distinct implementations of a Fraud Investigation Workbench, each scaling in complexity and feature set. Whether you need a simple local tool or a production-ready full-stack platform, there is a version tailored for you.

---

## 📂 Project Summaries

### 1. [Fraud-AI-Workbench-basic](./Fraud-AI-Workbench-basic)
The entry-level workbench focusing on simplicity and core features.
- **Goal**: Rapid prototyping and basic fraud analysis.
- **Key Features**: Schema-Grounded SQL RAG, Knowledge-Base (KB) chat, and supervised/unsupervised ML models (Random Forest, Isolation Forest).
- **Tech**: Streamlit, SQLite.
- **Docker**: `docker compose up --build`
- **Repo**: [yanhuo68/Fraud-AI-Workbench-basic](https://github.com/yanhuo68/Fraud-AI-Workbench-basic)

### 2. [Fraud-AI-Workbench-plus](./Fraud-AI-Workbench-plus)
An enhanced version of the basic workbench with refined UI and more analytical tools.
- **Goal**: Deeper investigation with autonomous agents and media tracking.
- **Key Features**: Autonomous ReAct Agents (LangGraph), Whisper-powered Media Transcription, Visual Execution Player for replay, and automated ERD generation (Mermaid).
- **Tech**: Streamlit, LangGraph, Graphviz.
- **Repo**: [yanhuo68/Fraud-AI-Workbench-plus](https://github.com/yanhuo68/Fraud-AI-Workbench-plus)

### 3. [Fraud-AI-Workbench-pro](./Fraud-AI-Workbench-pro)
A professional-grade, highly-scalable enterprise architecture.
- **Goal**: Production-ready, secure, distributed fraud analysis platform.
- **Key Features**: Graph RAG (Neo4j), Multimodal FAISS RAG, Admin RBAC Console, FastAPI Backend Router, API Hub, and Interactive visual Demos.
- **Tech**: Streamlit (Frontend), FastAPI (Backend), Neo4j, FAISS, SQLAlchemy, Ollama.
- **Repo**: [yanhuo68/Fraud-AI-Workbench-pro](https://github.com/yanhuo68/Fraud-AI-Workbench-pro)

### 4. [Fraud-AI-Workbench-plus-max](./Fraud-AI-Workbench-plus-max)
The most advanced experimental version featuring cutting-edge multi-agent techniques.
- **Goal**: High-fidelity fraud detection utilizing hybrid graph-based context.
- **Key Features**: Hybrid TF-IDF Graph RAG, SMOTE for imbalanced data, Risk Guideline auto-indexing, and dynamic agent logic maps.
- **Tech**: Streamlit, LangGraph, Sentence-Transformers, Imbalanced-learn.
- **Repo**: [yanhuo68/Fraud-AI-Workbench-plus-max](https://github.com/yanhuo68/Fraud-AI-Workbench-plus-max)

---

## 📊 Feature Comparison Matrix

| Feature | Basic | Plus | Pro | Plus-Max |
| :--- | :---: | :---: | :---: | :---: |
| **SQL RAG** | ✅ | ✅ | ✅ | ✅ |
| **KB Chat** | ✅ | ✅ | ✅ | ✅ |
| **ML Dashboard** | ✅ | ✅ | ✅ | ✅ (Advanced) |
| **ERD Generation** | ❌ | ✅ | ✅ | ✅ |
| **Architecture** | App | App | Full-Stack (API) | App |
| **Graph RAG** | ❌ | ❌ | ✅ (Neo4j) | ✅ (Hybrid) |
| **Multimodal RAG** | ❌ | ✅ (Whisper) | ✅ (Faiss/OCR) | ❌ |
| **Agent Workflows**| ❌ | ✅ | ❌ | ✅ |
| **RBAC / Security**| ❌ | ❌ | ✅ | ❌ |

---

## 🛠️ Quick Start

Each project has its own `README.md` with specific installation instructions. Generally, the setup involves:

1. **Install Dependencies**: `pip install -r requirements.txt` within the project folder.
2. **Environment Setup**: Create a `.env` file with your `OPENAI_API_KEY` or other provider keys.
3. **Launch**: Run `streamlit run dashboard.py` (or `app.py`).

For the **Pro** version, you will also need to start the FastAPI backend:
`uvicorn api.main:app --reload`

---

## 📋 Requirements

- **Python 3.11+**
- **LLM Access**: OpenAI, DeepSeek, or local models via Ollama/LM Studio.
- **System Tools**: `graphviz` (for ERD/Graph visualization).

---

## 🤝 Contributing

Feel free to explore each project and contribute improvements! Each workbench is designed to be modular and extensible.
