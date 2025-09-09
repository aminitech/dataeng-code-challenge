# Data Engineer Technical Challenge

## 🚀 Overview
For this challenge, we’re building a **Retrieval-Augmented Generation (RAG)** system to handle document ingestion, extract meaningful content, store it in structured formats, and make it queryable using LLMs.  

This challenge is a **simplified version** of that workflow. It’s not about building a production system — it’s about showing us how you think, code, and design scalable solutions.

We want to see your ability to:
- Write clean, modular Python code.
- Design and explain scalable data pipelines.
- Integrate with modern AI tools (LLMs).
- Communicate your decisions and trade-offs clearly.

⏱️ Timebox: Around **3 hours** (for a senior engineer).

---

## 🛠️ Part 1 – Implementation (Code)
Build a simple pipeline with the following steps:

1. **Ingestion** → Accept one or more PDF files as input.  
2. **Processing** → Extract and clean the text (basic normalization, chunking).  
3. **Storage** → Save the chunks in a structured format (JSON, CSV, SQLite, or Postgres).  
4. **Query Interface** → Allow a user to ask a question and retrieve relevant chunks using an **LLM integration**:  
   - Use either a hosted API (OpenAI, Anthropic, etc.) or a local LLM runtime ([Ollama](https://ollama.ai/)).  
   - Document the setup so we can reproduce your solution.  

👉 Mocking is acceptable where needed, but please include **at least one real LLM call** (API or local).

---

## 🏗️ Part 2 – Architecture & Scalability
Provide a simple **diagram + explanation** of how you’d scale this pipeline:
- Handling thousands of documents in parallel.  
- Using orchestration tools (e.g., Airflow) for scheduling/monitoring.  
- Integrating with cloud storage & warehouses (AWS S3, Redshift, BigQuery, etc.).  
- Exposing the query system via an API (e.g., FastAPI).  

---

## 📝 Part 3 – Documentation & Reflection
Alongside your code, add a short README or design note explaining:
- What you actually implemented vs. what you mocked.  
- Setup instructions so we can run your solution locally.  
- Improvements you’d make with more time (e.g., embeddings, knowledge graph, caching).  
- The reasoning behind your technical decisions.  

---

## ✅ What We’re Looking For
- **Code quality** → Clear, modular, with error handling and (if possible) simple tests.  
- **Data engineering best practices** → Thoughtful ETL/pipeline design, scalability, reproducibility.  
- **Architecture thinking** → Ability to explain design choices and extensions.  
- **Communication** → Clear documentation, easy-to-follow explanations.  

---

## 📦 Deliverables
Please submit:
- Your **code implementation** (in a GitHub repo or as a zip file).  
- A **README** (like this one) updated with your notes.  
- An **architecture diagram** (image, PDF, or link to draw.io / mermaid).  

---

Good luck — we’re excited to see your solution! ✨