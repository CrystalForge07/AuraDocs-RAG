# LangChain Documentation Helper

A RAG-based AI assistant that answers questions about LangChain documentation using document retrieval, vector search, and an LLM-powered agent.

## Features

- Crawls LangChain documentation using Tavily
- Splits documentation into smaller chunks
- Generates embeddings using Hugging Face
- Stores and retrieves vectors using Pinecone
- Uses LangChain agents for tool-based retrieval
- Uses Groq's `openai/gpt-oss-20b` model for answering questions
- Provides source references for retrieved documentation
- Streamlit interface for easy interaction

## Architecture

```text
LangChain Documentation
        ↓
   Tavily Crawl
        ↓
   Text Chunking
        ↓
 Hugging Face Embeddings
        ↓
      Pinecone
        ↓
   Retriever Tool
        ↓
 LangChain Agent
        ↓
      Groq LLM
        ↓
     Answer + Sources
        ↓
     Streamlit UI
```
# Tech stack
-Python
-LangChain
-LangChain Agents
-Tavily
-Pinecone
-Hugging Face Sentence Transformers
-Groq
-Streamlit
