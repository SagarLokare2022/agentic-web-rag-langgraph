<img width="309" height="432" alt="image" src="https://github.com/user-attachments/assets/a3759540-9fda-48dc-8efe-b52b282c66f9" />


# Agentic Web RAG (LangGraph + LangChain + OpenAI)

A simple **agentic Web RAG** project built with **LangGraph**:
- The agent **routes** the question:
  - **Direct Answer** (LLM only) for general questions
  - **RAG Answer** (Retriever + LLM) for doc/web-based questions
- When RAG is used, the response includes **source URLs**

## How it works

- **route** → decides whether to use retrieval (keyword-based router)
- **retrieve** → fetches relevant chunks from the indexed web pages
- **rag_answer** → answers using retrieved context + prints sources
- **direct_answer** → answers using LLM knowledge only


