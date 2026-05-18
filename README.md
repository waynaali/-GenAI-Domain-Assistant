# Week 9 & 10: GenAI Domain Assistant + RAG System (Gemini API Version)

This repository contains the implementation of conversational AI assistants and a Retrieval-Augmented Generation (RAG) system developed using the **Google Gemini API** in a Jupyter Notebook / Kaggle environment.

---

# Week 9: GenAI Domain Assistant

## Features Implemented

### Environment Setup
- Secure API key management using **Kaggle Secrets** / `.env` files
- Gemini API integration using the `google-generativeai` SDK

### Conversational Chatbot
- Multi-turn conversational chatbot using Gemini models
- Context-aware responses through persistent chat sessions

### Custom AI Personalities
- Domain-specific system prompts and guardrails
- Controlled assistant behavior for specialized tasks

---

## Domain-Specific Assistants

### HR Assistant
Handles employee-related queries such as:
- Vacation policies
- Remote work policies
- Insurance benefits
- 401(k) information

### Customer Support Assistant
A support chatbot for **TechShop** electronics retail:
- Return policies
- Shipping information
- Warranty handling
- Customer issue resolution

---

## Error & Quota Handling
Implemented exception handling for:
- Invalid API keys
- API quota exhaustion
- Rate limits (429 errors)
- Gemini API client/server errors

---

# Week 10: Retrieval-Augmented Generation (RAG)

## Features Implemented

### Document Processing
- Loaded documents from directory
- Parsed and processed text files

### Text Chunking
- Split documents into chunks (~500 characters)
- Preserved context for retrieval

### Retrieval System
Implemented:
- `simple_search()` retrieval function
- Keyword/context matching
- Top-k relevant chunk selection

### RAG Query Pipeline
Implemented:
- Context retrieval
- Prompt construction
- Gemini-powered answer generation
- Context-restricted answering

### Hallucination Prevention
If answer is unavailable in documents, system returns:
> `"Not found in documents"`

### RAG vs Non-RAG Comparison
Compared:
- Direct LLM responses
- Retrieval-augmented responses

Demonstrated improved factual grounding using RAG.

---

# Tech Stack

- Python 3.x
- Google Gemini API
- `google-generativeai`
- `langchain`
- `langchain-google-genai`
- `python-dotenv`
- Jupyter Notebook / Kaggle

---

# Models Used

- `gemini-pro`
- `gemini-1.5-pro`

---

# Key Concepts Covered

- Prompt Engineering
- Multi-turn Conversations
- Domain-Specific AI Assistants
- Retrieval-Augmented Generation (RAG)
- Document Chunking
- Context Injection
- Semantic Retrieval
- API Integration
- Error Handling
- Hallucination Reduction

---

# Example Capabilities

## HR Assistant
> "How many vacation days do employees get?"

## Customer Support Assistant
> "Can I return a laptop after 15 days?"

## RAG-Based QA
> Answers questions strictly from uploaded documents.

If information is unavailable:
> `"Not found in documents"`

---

# Deliverables Completed

- [x] Documents loaded from directory
- [x] Text split into chunks
- [x] Chunk preview generated
- [x] Retrieval system implemented
- [x] Tested retrieval queries
- [x] RAG query pipeline implemented
- [x] Document-grounded responses generated
- [x] Handled missing-context responses
- [x] Compared RAG vs non-RAG outputs
- [x] Gemini API integration completed
- [x] Error handling implemented
