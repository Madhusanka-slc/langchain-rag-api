
# LangChain RAG API

A **Retrieval-Augmented Generation (RAG) API** built with LangChain and FastAPI that enables intelligent chat with private knowledge sources using vector embeddings and semantic search, featuring rate limiting and secure API key authentication.

---

## Tech Stack

* **LangChain** – LLM orchestration and RAG pipeline
* **FastAPI** – REST API framework
* **OpenAI** – LLMs and embeddings
* **Upstash Vector** – Vector database for embeddings
* **Upstash Redis** – Rate limiting and activity tracking
* **LangServe** – Remote Runnable client

---

## Features

* **Retrieval-Augmented Generation** – Chat with your private documents using semantic search
* **Vector Embeddings** – Store and retrieve document embeddings with Upstash Vector
* **Rate Limiting** – API key-based rate limiting with Upstash Redis
* **REST API** – Production-ready FastAPI endpoints with LangServe
* **Interactive Notebooks** – Step-by-step Jupyter notebooks for learning
* **Secure by Design** – API key authentication and rate limit middleware

---

## Getting Started

Clone the repository:

```bash
git clone https://github.com/Madhusanka-slc/langchain-rag-api.git
cd langchain-rag-api
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Set up environment variables (create a `.env` file):

```env
OPENAI_API_KEY=your_openai_key
UPSTASH_VECTOR_URL=your_upstash_vector_url
UPSTASH_VECTOR_TOKEN=your_upstash_vector_token
UPSTASH_REDIS_URL=your_upstash_redis_url
```

Run the API:

```bash
uvicorn main:app --reload
```

Now the API will be running at `http://127.0.0.1:8000`. Explore the interactive docs at `/docs` and test the RAG chatbot endpoint.
