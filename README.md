# Context Agent AI

Context-aware RAG assistant for semantic retrieval, document understanding, and AI-powered contextual search using FastAPI, LangChain, and vector databases.

This project is designed to process documents, retrieve relevant contextual information using vector search, and generate structured AI-powered responses through Retrieval-Augmented Generation (RAG).

---

# Features

- RAG-based contextual retrieval
- Semantic document search using embeddings
- FastAPI backend APIs
- ChromaDB vector storage
- LangChain-powered orchestration
- Conversational memory support
- Structured JSON responses
- Multi-document ingestion pipeline

---

# Architecture Flow

```text
User Query
    ↓
Retriever
    ↓
ChromaDB Vector Search
    ↓
Context Assembly
    ↓
LLM Response Generation
    ↓
Structured Response
````

---

# Example Use Cases

* Document question answering
* Semantic search across large knowledge bases
* Context-aware AI assistants
* Content understanding and summarization
* AI-powered contextual retrieval systems

---

# Example JSON Output

```json
{
  "query": "Summarize the uploaded document",
  "summary": "The document explains how vector databases improve semantic retrieval in RAG systems.",
  "sources": ["example_document.txt"],
  "follow_up_questions": [
    "How does ChromaDB store embeddings?",
    "What is semantic retrieval?"
  ]
}
```

---

# Tech Stack

## AI / LLM Systems

* LangChain
* RAG (Retrieval-Augmented Generation)
* ChromaDB
* Vector Embeddings

## Backend

* FastAPI
* Python
* REST APIs

## Storage

* ChromaDB
* SQLite

---

# API Endpoints

## Chat Endpoint

```http
POST /api/v1/chat
```

Generate contextual AI responses using retrieved document data.

---

## Document Ingestion

```http
POST /api/v1/ingest
```

Upload and index documents into the vector database.

---

## Health Check

```http
GET /api/v1/health
```

Returns service health status.

---

# Project Structure

```text
context-agent-ai/
│
├── app/
├── data/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── start.py
└── README.md
```

---

# Setup

## Clone Repository

```bash
git clone https://github.com/N-Aryan/context-agent-ai.git
cd context-agent-ai
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Backend

```bash
python start.py
```

---

# Future Improvements

* Hybrid retrieval pipelines
* Persistent conversational memory
* Multi-user context support
* Additional vector database integrations
* Streaming AI responses

---

# License

MIT License

```
```
