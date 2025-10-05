A Hybrid Retrieval-Augmented Generation (RAG) System for Research Question Answering

## 🚀 Overview
This repository presents a **hybrid RAG system** that enables research-focused question answering by combining:
- **Local collection of research papers** (via Excel/PDF/links)
- **Online retrieval** (via Tavily API)
- **Contextual response generation** (using HuggingFace LLMs)

The system provides **concise answers with citations** from papers or online sources, making it ideal for academic exploration and literature surveys.

---

## ✨ Features
- 📄 Load research papers from Excel/URLs
- 🔎 Chunk & embed documents using `sentence-transformers`
- 🗂️ Build and persist a FAISS vector database
- 🌐 Retrieve from online sources with Tavily API
- 🧠 Generate contextual answers with HuggingFace LLMs (`flan-t5-large` by default)
- 📌 Cite sources for transparency
- 🖥️ Interactive Q&A mode in terminal

---

## 🛠️ Tech Stack
- **Python 3.10+**
- [LangChain](https://www.langchain.com/)  
- [FAISS](https://github.com/facebookresearch/faiss)  
- [HuggingFace Transformers](https://huggingface.co/transformers/)  
- [sentence-transformers](https://www.sbert.net/)  
- [PyMuPDF](https://pymupdf.readthedocs.io/en/latest/) (for PDFs)  
- [Tavily API](https://tavily.com/) (for online search)  

---
