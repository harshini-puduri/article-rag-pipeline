# Article Q&A with LangChain + OpenAI (RAG Pipeline)

This project builds a lightweight Retrieval-Augmented Generation (RAG) pipeline that can read a real article and answer questions based on its content.

It uses LangChain to:
- Scrape a public article (on Agentic AI)
- Split it into context-aware chunks
- Embed those chunks with OpenAI (`text-embedding-3-large`)
- Store them in a FAISS vector store
- Retrieve the most relevant chunks given a user query
- Pass those to GPT-4o to generate grounded, accurate answers

All responses are based directly on the article — no hallucinations.

---

### Stack
- LangChain
- OpenAI (Embeddings + GPT-4o)
- FAISS
- WebBaseLoader
- Python + `.env` for config

---

