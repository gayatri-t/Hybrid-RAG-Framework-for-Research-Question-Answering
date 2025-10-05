A Hybrid Retrieval-Augmented Generation (RAG) System for Research Question Answering

## 🚀 Overview

This repository contains an **advanced Hybrid RAG system** designed for **research-focused question answering**.  
It integrates **local academic papers** with **online retrieval** (via Tavily API) and applies **hybrid search (BM25 + FAISS)**, **cross-encoder reranking**, and **query caching** to generate **concise, cited answers** using HuggingFace LLMs.


The system provides **concise answers with citations** from papers or online sources, making it ideal for academic exploration and literature surveys.

---

## ✨ Key Features
- 📄 **Local Knowledge Base**: Load research papers from Excel (PDFs/links supported)
- 🔎 **Chunking & Embedding**: Split text and embed with `sentence-transformers`
- 🗂️ **FAISS Vector Store**: Persist embeddings for semantic search
- 📑 **BM25 Index**: Keyword-based retrieval for hybrid search
- 🤝 **Hybrid Search**: Combines BM25 + FAISS for more robust results
- 🎯 **Cross-Encoder Reranking**: Refines retrieved results with `ms-marco-MiniLM`
- 🌐 **Online Retrieval**: Integrates Tavily API for web sources
- 🧠 **LLM Answer Generation**: Uses HuggingFace LLMs (e.g., `LLaMA-3-8B-Instruct`)
- 📌 **Citation-Aware Responses**: Answers always include references
- 💾 **Query Caching**: Avoids recomputation for repeated queries
- 🖥️ **Interactive Terminal Q&A Mode**

---

## 🛠️ Tech Stack
- **Python 3.10+**
- [LangChain](https://www.langchain.com/) – orchestration
- [FAISS](https://github.com/facebookresearch/faiss) – vector search
- [BM25 (rank-bm25)](https://github.com/dorianbrown/rank_bm25) – keyword retrieval
- [sentence-transformers](https://www.sbert.net/) – embeddings
- [CrossEncoder](https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2) – reranking
- [HuggingFace Transformers](https://huggingface.co/transformers/) – LLM pipeline
- [Tavily API](https://tavily.com/) – online search
- [PyMuPDF](https://pymupdf.readthedocs.io/en/latest/) – PDF loader
- [Pandas](https://pandas.pydata.org/) – Excel ingestion

---
