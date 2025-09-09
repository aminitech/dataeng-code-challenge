# Data Engineer Technical Challenge

## Context
Amini is building a **Retrieval-Augmented Generation (RAG)** system for ingesting documents, extracting content, storing it in a structured form, and making it available for LLM-powered queries. Your challenge is to implement a simplified version of this pipeline.

The goal is **not** to build a production-ready system, but to demonstrate your ability to:
- Write clean and modular code in Python.
- Design and document scalable data pipelines.
- Integrate modern AI capabilities (LLMs).
- Communicate decisions, trade-offs, and potential improvements.

⏱️ Estimated time: ~3 hours for a senior engineer.

---

### Part 1 – Implementation (Code)
Implement a simplified pipeline that:

1. **Ingestion**: Accepts one or more PDF files as input.  
2. **Processing**: Extracts and cleans text (basic normalization, splitting into chunks).  
3. **Storage**: Saves the chunks in a structured format (e.g., JSON, CSV, SQLite, or Postgres).  
4. **Query Interface**: Enables the user to ask a question and retrieve relevant chunks using a **LLM integration**:  
   - You may use a hosted API (e.g., OpenAI, Anthropic, etc.) or a **local LLM runtime** (e.g., [Ollama](https://ollama.ai/)).  
   - Document the setup and steps so we can reproduce your solution on our side.  

👉 Mocking is allowed where needed, but **at least one working LLM call** (local or API-based) should be demonstrated.

---

### Part 2 – Architecture & Scalability
Deliver a simple diagram + explanation of how this pipeline could be scaled:
- Handling thousands of documents in parallel.  
- Using orchestration tools (e.g., Airflow) to schedule/monitor.  
- Leveraging cloud storage and data warehouses (e.g., AWS S3, Redshift, BigQuery).  
- Exposing the query system as an API (e.g., FastAPI).  

---

### Part 3 – Documentation & Reflection
Provide a short README or design note covering:
- What you implemented and what you mocked.  
- Setup instructions so we can run your solution locally.  
- Possible improvements with more time (e.g., embeddings search, knowledge graph integration, caching).  
- Trade-offs and reasoning behind your technical choices.  

---

## Evaluation Criteria
- **Code quality**: clarity, modularity, basic error handling, tests if possible.  
- **Engineering practices**: data pipeline design, scalability considerations, reproducibility.  
- **Architecture thinking**: ability to explain design choices and future extensions.  
- **Communication**: clarity of documentation and explanation of trade-offs.  

---

## Deliverables
- Code implementation (in a GitHub repo or zip file).  
- A README (like this) updated with your notes.  
- Architecture diagram (can be an image or a simple draw.io / mermaid diagram).  

Good luck – we’re excited to see your solution!