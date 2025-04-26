# Simple GenAI Application — Exploring Agentic AI with LangChain + OpenAI

Welcome to my little experiment in making GenAI more useful, searchable, and context-aware!
This project started as a curiosity:  
> *Can I build something that reads an article, understands it, and answers my questions like a smart assistant?*

## 🧠 What this project does?

This notebook pulls together the core pieces of a Retrieval-Augmented Generation (RAG) pipeline:

- Scrapes a real article on **Agentic AI** from [Adams Street Partners](https://www.adamsstreetpartners.com/insights/the-next-frontier-the-rise-of-agentic-ai/)
- Breaks the content into meaningful chunks using LangChain’s recursive text splitter
- Creates vector embeddings using OpenAI’s `text-embedding-3-large`
- Stores those vectors locally using **FAISS**
- Lets you ask questions, retrieves the best-matching content, and then uses **GPT-4o** to answer your query — grounded in that content

Think of it as a mini research assistant trained on one article.

---

## Example

**You ask:**  
> *"What are some emerging use cases for agentic AI?"*

**It replies:**  
> "Agentic AI is being used in procurement, sales support, and customer service. It enables decision-making workflows, automates repetitive tasks, and allows human teams to focus on high-value strategy."

And it tells you *exactly* which part of the article that info came from. No hallucinations. Just context-based responses.

---

## 🛠️ Stack

- 🧱 **LangChain** – for orchestration, parsing, chunking
- 💬 **OpenAI (GPT-4o)** – for generating natural answers
- 🧠 **FAISS** – for fast, local semantic search
- 🌐 **WebBaseLoader** – scrapes the article
- 📦 **.env** – stores your API keys securely

---

## 🚀 How to run it

1. **Clone the repo:**

```bash
git clone git@github.com:harshini-puduri/Simple-GenAI-application.git
cd Simple-GenAI-application

