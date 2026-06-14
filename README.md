# PDF RAG App

A Retrieval-Augmented Generation (RAG) application that enables users to query PDF documents using Large Language Models. The application extracts content from PDFs, generates embeddings, stores them in a vector database, and retrieves relevant context to answer user questions accurately.

## 🚀 Features

* PDF document ingestion
* Text chunking and preprocessing
* Embedding generation
* Vector database storage
* Semantic similarity search
* Context-aware question answering
* Local LLM integration with Ollama
* Docker support

## 🛠️ Tech Stack

* Python
* LangChain
* Ollama
* ChromaDB / Vector Store
* PyPDFLoader
* Jupyter Notebook
* Docker

## 📂 Project Structure

```text
PDF_RAG_APP/
│
├── RAG_app/
│   ├── Docs/                 # Source PDF documents
│   ├── Vector/               # Vector database storage
│   ├── app.ipynb             # Main RAG implementation
│   └── rag_with_pdf.ipynb    # Development notebook
│
├── docker-compose.yaml       # Docker configuration
├── pyproject.toml            # Project dependencies
├── uv.lock                   # Dependency lock file
├── .gitignore
└── README.md
```

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/pdf-rag-app.git
cd pdf-rag-app
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Environment

Windows:

```bash
.venv\Scripts\activate
```

Linux/Mac:

```bash
source .venv/bin/activate
```

### Install Dependencies

Using uv:

```bash
uv sync
```

Or using pip:

```bash
pip install -r requirements.txt
```

## 🦙 Setup Ollama

Install Ollama and pull a model:

```bash
ollama pull llama3
```

Verify installation:

```bash
ollama list
```

## ▶️ Running the Project

Open and run:

```text
RAG_app/app.ipynb
```

or

```text
RAG_app/rag_with_pdf.ipynb
```

Execute the notebook cells sequentially to:

1. Load PDF documents
2. Split documents into chunks
3. Create embeddings
4. Store vectors
5. Query the document
6. Generate answers using the LLM

## 💡 Example Questions

* Summarize the uploaded document.
* What is the main topic discussed?
* Explain the key concepts.
* Extract important points from Chapter 1.
* What conclusions does the document provide?

## 🔄 RAG Workflow

```text
PDF
 │
 ▼
Document Loader
 │
 ▼
Text Splitter
 │
 ▼
Embeddings
 │
 ▼
Vector Store
 │
 ▼
Retriever
 │
 ▼
LLM (Ollama)
 │
 ▼
Answer Generation
```

## 🎯 Learning Outcomes

This project demonstrates:

* Retrieval-Augmented Generation (RAG)
* Vector Databases
* Embeddings
* Semantic Search
* LangChain Pipelines
* Local LLM Deployment
* Document Question Answering

## 🔮 Future Improvements

* Streamlit Web Interface
* Multiple PDF Support
* Chat History
* Source Citations
* Hybrid Search
* Deployment on Cloud


