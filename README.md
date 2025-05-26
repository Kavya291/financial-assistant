# FinSight: Agentic AI-Powered Financial Assistant

**FinSight** is an intelligent, multi-agent financial assistant designed to deliver real-time market insights through natural language interaction. It integrates structured data from financial APIs, unstructured data from regulatory filings and news, and large language models (LLMs) to produce meaningful summaries, forecasts, and financial briefings. The system supports both voice and text-based interactions through a unified interface.

This project demonstrates the power of agentic AI in finance, combining retrieval-augmented generation (RAG), document analysis, API-driven data ingestion, and voice interfaces within a modular, microservice-based architecture.

---

## Key Features

- Real-time financial data retrieval via external APIs
- Automated ingestion and summarization of company filings (e.g., 10-Ks)
- Intelligent responses generated using large language models
- Semantic search with vector embeddings for contextual accuracy
- Voice input (speech-to-text) and audio response (text-to-speech)
- Web-based user interface built with Streamlit

---

## Architecture Overview

The system is designed using a modular, multi-agent architecture. Each agent performs a specific function and communicates through a centralized orchestrator.

**Core Components:**

- **Data Ingestion Agent**: Pulls real-time stock and financial data from external APIs such as Yahoo Finance or AlphaVantage.
- **Web Scraping Agent**: Extracts unstructured data from financial news and regulatory filings.
- **Retriever Agent**: Embeds and stores documents using vector databases (e.g., FAISS) and retrieves context using semantic search.
- **Language Agent**: Generates responses using LLMs via retrieval-augmented generation.
- **Voice Agent**: Handles speech-to-text and text-to-speech processing for multimodal interaction.
- **Orchestrator**: FastAPI-based controller that routes user queries across the agents and returns the final response.
- **Frontend Interface**: Built using Streamlit, allowing users to interact via voice or text.

---

## Technology Stack

- **Programming Language**: Python 3.10+
- **Frameworks**: FastAPI, Streamlit, LangChain
- **LLMs**: OpenAI GPT-3.5 or Claude 3 (via LangChain)
- **Data Retrieval**: yfinance, AlphaVantage, BeautifulSoup
- **Embedding & Vector Search**: OpenAI Embeddings, FAISS
- **Voice Processing**: whisper, speechrecognition, pyttsx3
- **Containerization**: Docker

---


