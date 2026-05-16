# Week 9: GenAI Domain Assistant (Gemini API Version)

This repository contains the implementation of a Python-based conversational AI chatbot developed using the **Google Gemini API** (via the `google-genai` SDK) and managed within a Jupyter Notebook / Kaggle environment. 

## Features Implemented
* **Environment Setup:** Securely managed API tokens using `.env` files / Kaggle Secrets.
* **Basic Chatbot Loop:** Handles multi-turn dialogues seamlessly using Gemini's built-in chat sessions (`client.chats.create`).
* **Custom System Prompts:** Structured AI personalities and guardrails via custom system instructions.
* **Domain-Specific Assistants:** * **HR Assistant:** Specialized in tech company policies (vacation, insurance, 401k).
  * **Customer Support Bot:** An empathetic agent for 'TechShop' electronics retail handling returns, warranty, and shipping queries.
* **Error & Quota Handling:** Robust exception layers (`ClientError` and `ServerError`) to gracefully handle API rate limits (429 errors).

## Tech Stack
* Python 3.x
* Google Gemini API (`gemini-2.5-flash`)
* `google-genai` SDK & `python-dotenv`
