# Week 9–12: GenAI Domain Assistant + Advanced RAG System (Gemini API Version)

This repository contains the implementation of conversational AI assistants and advanced Retrieval-Augmented Generation (RAG) systems developed using the **Google Gemini API**, **LangChain**, **ChromaDB**, and **Streamlit**.

The project evolved from basic conversational AI systems into fully interactive document-grounded assistants with vector databases, semantic retrieval, memory-aware conversations, and web-based deployment.

---

# Week 9: GenAI Domain Assistant

## Features Implemented

### Environment Setup

* Secure API key management using:

  * Kaggle Secrets
  * `.env` files
* Gemini API integration using:

  * `google-generativeai`
  * `langchain-google-genai`

---

## Conversational Chatbot

Implemented:

* Multi-turn conversational chatbot
* Persistent chat sessions
* Context-aware dialogue handling
* Gemini-powered response generation

---

## Custom AI Personalities

Created specialized assistants using:

* System prompts
* Prompt engineering
* Guardrails
* Controlled response formatting

---

# Domain-Specific Assistants

## HR Assistant

Handles employee-related queries such as:

* Vacation policies
* Remote work policies
* Insurance benefits
* 401(k) information
* Employee onboarding

---

## Customer Support Assistant

Built a support chatbot for **TechShop** electronics retail.

Capabilities:

* Return policy handling
* Warranty support
* Shipping assistance
* Refund guidance
* Customer issue resolution

---

# Error & Quota Handling

Implemented robust exception handling for:

* Invalid API keys
* API quota exhaustion
* Rate limits (429 errors)
* Gemini client/server errors
* Missing environment variables
* Invalid requests

---

# Week 10: Retrieval-Augmented Generation (RAG)

## Document Processing

Implemented:

* Directory-based document loading
* Text file parsing
* Automated preprocessing pipeline

---

## Text Chunking

Implemented:

* Recursive text splitting
* Chunk overlap handling
* Context-preserving chunk generation
* ~500-character semantic chunks

---

## Retrieval System

Built:

* `simple_search()` retrieval function
* Top-k retrieval pipeline
* Context matching
* Semantic search workflow

---

## RAG Query Pipeline

Implemented:

* Context retrieval
* Prompt construction
* Gemini-powered grounded responses
* Context injection pipeline

---

## Hallucination Prevention

If information is unavailable in documents, system responds:

> `"Not found in documents"`

Implemented strict context-restricted answering.

---

## RAG vs Non-RAG Comparison

Compared:

* Direct LLM responses
* Retrieval-augmented responses

Demonstrated:

* Reduced hallucinations
* Better factual grounding
* Improved domain accuracy

---

# Week 11: Vector Database + Semantic Search Upgrade

## ChromaDB Integration

Integrated:

* Persistent ChromaDB vector database
* Local vector storage
* Semantic embedding search

---

## Embedding Pipeline

Implemented:

* SentenceTransformer embeddings
* `all-MiniLM-L6-v2` embedding model
* Semantic similarity search
* Vector indexing pipeline

---

## Advanced Retrieval

Upgraded retrieval system with:

* Embedding-based semantic retrieval
* Similarity scoring
* Top-k ranked retrieval
* Faster document lookup

---

## LangChain Integration

Integrated LangChain for:

* Prompt templating
* LLM abstraction
* Retrieval workflows
* RAG orchestration

---

## Persistent Knowledge Base

Implemented:

* Persistent vector database storage
* Reloadable collections
* Cached embeddings
* Efficient document reuse

---

# Week 12: Streamlit Deployment + Interactive AI Assistant

## Streamlit Web Application

Developed a full interactive web app using Streamlit.

Features:

* Chat interface
* Real-time AI responses
* Sidebar controls
* Conversation history
* Interactive UI components

---

## Session State Management

Implemented:

* Persistent conversation memory
* Chat history tracking
* Dynamic UI updates
* Stateful interactions

---

## Interactive RAG Assistant

Users can:

* Ask document-related questions
* Retrieve grounded answers
* Interact with AI in real time
* Query indexed company knowledge

---

## Cached Resource Optimization

Optimized performance using:

* `@st.cache_resource`
* Cached model loading
* Cached ChromaDB initialization
* Reduced API overhead

---

## Error Handling & Stability

Improved robustness with:

* Global exception handling
* User-friendly error messages
* Missing database detection
* API failure recovery

---

# Tech Stack

* Python 3.x
* Google Gemini API
* Streamlit
* ChromaDB
* LangChain
* LangChain Google GenAI
* SentenceTransformers
* python-dotenv
* Jupyter Notebook
* Kaggle
* VS Code

---

# Models Used

## LLMs

* `gemini-pro`
* `gemini-1.5-pro`
* `gemini-1.5-flash`

---

## Embedding Models

* `all-MiniLM-L6-v2`

---

# Key Concepts Covered

* Prompt Engineering
* Multi-turn Conversations
* Domain-Specific AI Assistants
* Retrieval-Augmented Generation (RAG)
* Semantic Search
* Vector Databases
* ChromaDB
* Embeddings
* LangChain Pipelines
* Streamlit Deployment
* Context Injection
* Document Chunking
* Persistent Memory
* API Integration
* Error Handling
* Hallucination Reduction
* Semantic Retrieval
* Conversational AI Systems

---

# Example Capabilities

## HR Assistant

> "How many vacation days do employees get?"

---

## Customer Support Assistant

> "Can I return a laptop after 15 days?"

---

## RAG-Based QA

> Answers questions strictly from uploaded documents.

If information is unavailable:

> `"Not found in documents"`

---

# Deliverables Completed

* [x] Documents loaded from directory
* [x] Text preprocessing pipeline implemented
* [x] Recursive text chunking completed
* [x] Chunk preview generation
* [x] Semantic embedding pipeline created
* [x] ChromaDB vector database integrated
* [x] Persistent vector storage implemented
* [x] Retrieval system implemented
* [x] Semantic similarity search added
* [x] Tested retrieval queries
* [x] RAG query pipeline implemented
* [x] Gemini-powered grounded responses generated
* [x] Hallucination prevention implemented
* [x] RAG vs non-RAG comparison completed
* [x] Streamlit web application developed
* [x] Interactive chatbot interface created
* [x] Session-state conversation memory implemented
* [x] Sidebar analytics added
* [x] Cached resource optimization completed
* [x] Gemini API integration completed
* [x] LangChain integration completed
* [x] Error handling implemented
* [x] End-to-end conversational RAG assistant deployed
