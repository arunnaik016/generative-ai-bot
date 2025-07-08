# generative-ai-bot

# 🦊 Aesop's Fables AI Chatbot using Groq

An interactive, intelligent chatbot built using **Groq AI** that deeply understands and interacts with the content of a 100+ page document – *Aesop’s Fables* 📘. Ask questions, get answers, hear spoken responses, and even see simplified explanations – all powered by cutting-edge language models and vector search.

---

## 🚀 Features

- 💬 **Ask Questions** from any part of the document
- 📢 **Text-to-Speech (TTS)**: Click to hear the answer aloud
- 📝 **Summarize Stories** with one click
- 🧒 **Explain Like I'm 5**: Simplified, beginner-friendly responses
- ⚡ **Ultra-fast inference** powered by Groq LLM (LLaMA3)

---

## 📄 Document Used

> **Aesop’s Fables – Project Gutenberg**  
> Total Pages: 100+  
> [Download PDF Link](https://www.gutenberg.org/ebooks/11339)

---

## 🧠 Tech Stack

| Component        | Library / Tool |
|------------------|----------------|
| LLM Inference    | `Groq API` via `LangChain` |
| Embeddings       | `SentenceTransformer (all-MiniLM-L6-v2)` |
| Vector Store     | `FAISS` |
| Chunking         | `LangChain Text Splitter` |
| Document Parsing | `PyMuPDF` |
| Frontend         | `Google Colab` + `ipywidgets` |
| TTS              | `gTTS` (Google Text-to-Speech) |

---

## 📊 Architecture

```text
PDF → Extract Text → Chunk → Embed → Vector Store (FAISS) → Groq LLM
                                                       ↓
                              Retrieval + Answering + Interactive UI
