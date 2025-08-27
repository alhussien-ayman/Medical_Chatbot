# Medical_Chatbot

A Flask-based chatbot for medical questions that uses **LangChain**, **Pinecone**, and **Hugging Face embeddings** to retrieve and answer questions from medical documents.

---

## Features

- Question-answering on medical PDFs
- Retrieval-Augmented Generation (RAG) using LangChain
- Pinecone vector database for fast document retrieval
- Hugging Face embeddings (`sentence-transformers/all-MiniLM-L6-v2`)
- OpenAI or Hugging Face LLM for responses
- Web-based chat interface with Flask

---

## Requirements

- Python 3.10+
- Pip package manager

### Python Libraries

Install all dependencies:

```bash
pip install flask langchain langchain_community langchain-pinecone langchain-openai pinecone-client sentence-transformers transformers huggingface-hub python-dotenv

### File structure

Medical_Chatbot/
│
├─ data/                     # PDF documents
├─ templates/
│   └─ chat.html              # Chat interface
├─ src/
│   ├─ helper.py              # Functions to load PDFs, embeddings, Pinecone
│   └─ prompt.py              # System prompts for LangChain
├─ store_index.py             # Script to generate embeddings and store in Pinecone
├─ app.py                     # Flask application
├─ requirements.txt           # Python dependencies (optional)
└─ README.md


