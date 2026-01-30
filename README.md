# Controllable RAG Agent (Document Question Answering)

This repository contains an implementation of a **Controllable Retrieval-Augmented Generation (RAG) Agent** for grounded question answering over documents.

The project demonstrates an agentic workflow where retrieval and reasoning are structured into multiple stages, enabling more transparent and controllable responses compared to standard single-step RAG pipelines.

---

## Overview

Retrieval-Augmented Generation (RAG) combines:

- **Document Retrieval** (vector search over embedded content)
- **Large Language Model Generation** (grounded answers based on retrieved context)

This repository extends the idea further by using a **controllable agent pipeline**, where the system retrieves from different sources such as:

- document chunks  
- extracted quotes  
- summarized chapters  

and then produces a final answer with better grounding.

---

## Key Components

- **Multi-stage retrieval workflow**
- **Vector store integration** (FAISS-based indexes included)
- **Agent-style controllable execution**
- **Notebook-based demonstration**
- **Graph visualization of the pipeline**

---

## Project Structure

- `sophisticated_rag_agent_harry_potter.ipynb`  
  Main notebook demonstrating the controllable RAG agent

- `simulate_agent.py`  
  Script-based agent simulation

- `functions_for_pipeline.py` / `helper_functions.py`  
  Core pipeline utilities

- `assets/`  
  Precomputed vector stores (FAISS indexes)

- `graphs/`  
  Workflow and execution graphs

---

## Requirements

Python 3.10+ is recommended.

Install dependencies:

```bash
pip install -r requirements.txt
