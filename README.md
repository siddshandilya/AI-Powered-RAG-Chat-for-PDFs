# AI-Powered-RAG-Chat-for-PDFs
AI-powered RAG chatbot for PDFs built with Streamlit, LlamaIndex, and Nebius AI's Qwen3. Upload documents, perform semantic search, and receive accurate, context-aware answers through an interactive chat interface.

# 🚀 DocWhisper – AI-Powered RAG Chat for PDFs

> **An enterprise-grade Retrieval-Augmented Generation (RAG) application that enables users to chat with PDF documents using state-of-the-art Large Language Models, semantic retrieval, and an intuitive Streamlit interface.**

Built with **Streamlit**, **LlamaIndex**, **Nebius AI**, and **Qwen3-235B-A22B**, this project demonstrates a production-style RAG pipeline featuring document ingestion, semantic search, context retrieval, and transparent AI reasoning.

---

## ✨ Demo

<p align="center">
  <img src="assets/demo.gif" width="900" alt="Application Demo">
</p>



---

# 📖 Overview

Traditional LLMs are limited by their training data and cannot reliably answer questions about private or newly uploaded documents.

This application solves that problem using **Retrieval-Augmented Generation (RAG)**.

Instead of relying solely on the model's memory, it:

- 📄 Reads uploaded PDF documents
- 🔍 Converts them into semantic embeddings
- 📚 Retrieves the most relevant document chunks
- 🧠 Uses those chunks as context for the LLM
- 💬 Generates accurate, grounded responses

The result is a fast, intelligent document assistant capable of answering questions directly from uploaded PDFs.

---

# ✨ Features

- 📄 Upload and chat with PDF documents
- 🤖 Powered by **Qwen3-235B-A22B**
- 🔍 Semantic Retrieval using **LlamaIndex**
- 🎯 High-quality embeddings with **BAAI/bge-en-icl**
- ⚡ Real-time document indexing
- 💬 Modern conversational interface
- 🧠 Transparent reasoning display
- 📑 PDF preview inside the application
- 🔄 Conversation history support
- 🗑️ One-click chat reset
- 🏗️ Modular architecture for easy extension

---

# 🏛️ System Architecture

```text
                  +--------------------+
                  |    Upload PDF      |
                  +---------+----------+
                            |
                            ▼
                +----------------------+
                | Document Processing  |
                |     (PyPDF2)         |
                +----------+-----------+
                           |
                           ▼
               +------------------------+
               |   LlamaIndex Parser    |
               +-----------+------------+
                           |
                           ▼
              +-------------------------+
              | Embedding Generation    |
              | BAAI/bge-en-icl         |
              +-----------+-------------+
                          |
                          ▼
              +-------------------------+
              | Vector Index Creation   |
              +-----------+-------------+
                          |
                          ▼
                 User Question
                          |
                          ▼
              +-------------------------+
              | Semantic Retrieval      |
              +-----------+-------------+
                          |
                          ▼
              +-------------------------+
              | Qwen3-235B-A22B LLM     |
              +-----------+-------------+
                          |
                          ▼
                 AI Generated Answer
```

---

# 🛠️ Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | Streamlit |
| LLM | Qwen3-235B-A22B |
| Alternative Model | DeepSeek-V3 |
| RAG Framework | LlamaIndex |
| Embedding Model | BAAI/bge-en-icl |
| PDF Processing | PyPDF2 |
| Vector Search | LlamaIndex Vector Store |
| Language | Python |

---

# 📂 Project Structure

```text
.
├── main.py
├── requirements.txt
├── assets/
│   ├── demo.gif
│   └── screenshots/
├── utils/
├── data/
├── README.md
└── .env
```

---

# ⚙️ Installation

## Clone the repository

```bash
git clone https://github.com/yourusername/docwhisper.git

cd docwhisper
```

## Create a virtual environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

## Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file.

```env
NEBIUS_API_KEY=your_api_key_here
```

---

# ▶️ Running the Application

```bash
streamlit run main.py
```

Open

```
http://localhost:8501
```

---

# 💻 Usage

### Step 1

Upload a PDF document from the sidebar.

---

### Step 2

The application automatically

- extracts text
- creates embeddings
- builds a searchable vector index

---

### Step 3

Ask questions naturally.

Example:

> What is the main objective of this report?

> Summarize the executive summary.

> Explain page 14 in simple terms.

> What are the key recommendations?

---

### Step 4

View

- Retrieved context
- AI reasoning
- Final response

all within the chat interface.

---

# 🧠 RAG Pipeline

```text
PDF Upload
      │
      ▼
Text Extraction
      │
      ▼
Chunking
      │
      ▼
Embedding Generation
      │
      ▼
Vector Index
      │
      ▼
Semantic Retrieval
      │
      ▼
LLM (Qwen3)
      │
      ▼
Grounded Response
```

---

# 🌟 Why This Project?

Unlike a standard chatbot, this application delivers:

- Hallucination reduction through retrieval
- Context-aware responses
- Document-grounded answers
- Semantic search instead of keyword matching
- Transparent reasoning for improved trust
- Modular RAG architecture suitable for production systems

---


