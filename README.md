#  ChatPDF RAG System

## Overview
This project implements a **Retrieval-Augmented Generation (RAG)** system that allows users to ask questions from a PDF document and receive **grounded, context-based answers**.

The system combines:
- Semantic search (FAISS)
- Embeddings (Sentence Transformers)
- LLM (OpenAI)

---

## 🧠 How It Works

Pipeline:
PDF → Chunking → Embeddings → FAISS → Retrieval → LLM → Answer


1. PDF is loaded and split into chunks  
2. Each chunk is converted into embeddings  
3. FAISS stores embeddings for fast similarity search  
4. User query is embedded and matched with relevant chunks  
5. LLM generates answer based only on retrieved context  

---

##  Features

-  PDF-based question answering  
-  Semantic search (not keyword-based)  
-  Context-aware responses  
-  Reduced hallucination (grounded answers)  
-  CLI-based interaction  

---

##  Tech Stack

- Python  
- LangChain  
- FAISS  
- Sentence Transformers (MiniLM)  
- OpenAI API  

---

##  Installation

```bash
pip install -r requirements.txt
---


