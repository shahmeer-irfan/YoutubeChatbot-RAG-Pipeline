# 🎥 YouTube Chatbot – RAG-Based Q&A System

This is a simple **RAG (Retrieval-Augmented Generation)** chatbot designed to answer user questions based on YouTube video transcripts. It uses an open-source LLM via OpenRouter and retrieves relevant transcript chunks using vector search.

## 🚀 Current Features

- Extracts transcripts from YouTube videos
- Splits and embeds text using open-source embedding models (e.g., HuggingFace)
- Stores embeddings in a local vector store (e.g., FAISS)
- Retrieves relevant context using similarity search
- Uses LLMs (like Mixtral or DeepSeek) to answer questions from the retrieved context
- Simple chain combining prompt template + retrieval + LLM + parsing

## 📦 Tech Stack

- Python (LangChain)
- OpenRouter (LLM inference)
- HuggingFace (Embeddings)
- FAISS (Vector storage)
- YouTube Transcript API

---

## 🛠️ Planned Improvements

Below are enhancements planned for the next version of the chatbot:

### 1. UI Enhancement
- Build a cleaner, more intuitive user interface using Streamlit or Gradio

### 2. Evaluation
- Integrate with **LangSmith** for RAG pipeline monitoring
- Add benchmarks to evaluate accuracy and factuality

### 3. Indexing
- Improve document ingestion pipeline
- Add advanced text splitting (by topics, timestamps, etc.)
- Move to cloud-based vector stores like Qdrant, Weaviate, or Pinecone

### 4. Retrieval

#### a. Pre-Retrieval
- Query rewriting using an LLM
- Multi-query generation for better coverage
- Domain-aware routing to target specific documents

#### b. During Retrieval
- MMR (Maximal Marginal Relevance) for diversity
- Hybrid retrieval (dense + sparse search)
- LLM-based reranking of retrieved results

#### c. Post-Retrieval
- Contextual compression to reduce token count while preserving meaning

### 5. Augmentation
- Prompt templating for consistent LLM input formatting
- Answer grounding to highlight the source of each answer
- Context window optimization for long transcripts

### 6. Generation
- Include citations in generated answers
- Add guardrails to reduce hallucination and maintain tone

### 7. System Design
- Move towards a multimodal architecture (text + image support)
- Add memory-based conversation history
- Explore agentic planning and tool use (ReAct-style agents)

---

## 🧑‍💻 Author

**Shahmeer Irfan**  
AI engineer in progress — focused on LLMs, RAG systems, and building practical AI tools.
