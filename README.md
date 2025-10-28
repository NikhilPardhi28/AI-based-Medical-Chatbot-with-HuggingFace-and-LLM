# 🩺 AROGYABOT
**Artificial Intelligence Diagnostic Bot using Machine Learning**

Arogyabot is an AI-powered chatbot designed to intelligently answer medical queries by analyzing and reasoning over user-uploaded medical documents. It integrates document parsing, vector-based semantic search, and a large language model (LLM) to deliver accurate, contextual answers — improving healthcare information accessibility and patient understanding.

---

## 🚀 Project Overview

Arogyabot enables users to upload medical PDF documents and query them conversationally.  
The system retrieves the most relevant sections using semantic similarity (FAISS) and generates a natural-language response using an LLM (Mistral).  
This helps medical professionals, students, and patients quickly extract insights from complex medical texts.

---

## 🧩 Features

✅ Upload and parse medical PDF documents  
✅ Automatic text chunking and preprocessing  
✅ Embedding generation for semantic understanding  
✅ Vector storage using FAISS for fast retrieval  
✅ Semantic search with top-K relevant document ranking  
✅ LLM (Mistral)–powered answer generation  
✅ Streamlit web interface for interactive chat and document management  
✅ Domain-specific embeddings using BioBERT for biomedical context  

---

## 🧠 System Architecture

[PDF Upload] → [Text Extraction] → [Chunking] → [Embeddings] → [FAISS Vector Store]
↑
|
[Question Embedding]
|
[Semantic Search → Top-K Chunks]
|
[Mistral LLM + Retrieved Context → Answer]
|
[Streamlit Chat UI]

yaml
Copy code

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend / UI | Streamlit |
| Backend | Python |
| Vector Store | FAISS |
| LLM | Mistral |
| Embeddings | BioBERT / Sentence Transformers |
| Libraries | `transformers`, `faiss-cpu`, `streamlit`, `pdfplumber`, `torch`, `langchain`, `tqdm` |

---

# README: Setting Up Your Environment with Pipenv

## Prerequisite: Install Pipenv
Follow the official Pipenv installation guide to set up Pipenv on your system:  
[Install Pipenv Documentation](https://pipenv.pypa.io/en/latest/installation.html)

---

## Steps to Set Up the Environment

### Install Required Packages
Run the following commands in your terminal (assuming Pipenv is already installed):

```bash
pipenv install langchain langchain_community langchain_huggingface faiss-cpu pypdf
pipenv install huggingface_hub
pipenv install streamlit



