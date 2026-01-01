![image](https://github.com/....png)

# Agentic Web RAG (LangGraph + LangChain + OpenAI)

![LangGraph Flow](assets/langgraph-flow.png)

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


