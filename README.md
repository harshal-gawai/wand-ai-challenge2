# Challenge 2 — AI-Powered Knowledge Base Search & Enrichment

##  Overview
This project implements an **AI-powered RAG (Retrieval-Augmented Generation)** pipeline that allows users to upload multiple documents, ask natural-language questions, receive grounded answers, detect missing information, and get enrichment suggestions.

It fulfills the **"AI-Powered Knowledge Base Search & Enrichment"** challenge by combining classical retrieval with an open-source LLM (Qwen-2.5-Instruct) for answer generation.

---

##  Features
- **Compressed Corpus** – All documents are provided inside `corpus.tar.xz`.  
- **Document Parsing** – Supports PDF and TXT files after extraction.  
- **Chunking** – Splits long documents into smaller overlapping pieces for efficient search.  
- **Retrieval Engine** – Uses TF-IDF similarity to find the most relevant chunks.  
- **AI Generation** – Integrates **Qwen-2.5-Instruct** for context-aware answers.  
- **Completeness Check** – Measures confidence and flags missing or uncertain info.  
- **Enrichment Suggestions** – Recommends what new data to add for better coverage.  
- **Structured Output** – Returns clean JSON with `answer`, `confidence`, `missing_info`, and `sources`.

---

##  Corpus Setup
Before running the notebook, extract the compressed corpus archive:
```bash
tar -xvf corpus.tar.xz
