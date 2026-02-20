# intelligent-warehouse-inventory-application

🏭 Warehouse AI Dashboard Streamlit + LangChain + Ollama + ChromaDB +
Animated Analytics

------------------------------------------------------------------------

PROJECT OVERVIEW The Warehouse AI Dashboard is an intelligent warehouse
management system powered by: - Local LLM using Ollama - Vector search
using ChromaDB - Retrieval-Augmented Generation (RAG) - Interactive
analytics dashboard - Animated futuristic UI with Streamlit - GPT
Accuracy scoring system

This project enables real-time querying of warehouse inventory and
shipment data using AI while ensuring no hallucinations and strictly
using available data.

------------------------------------------------------------------------

KEY FEATURES

AI-Powered Assistant Modes - Inventory Assistant - Shipment Assistant -
Multi-Task Assistant

Smart Data Upload - Upload CSV or Excel inventory files - Automatic
preview & validation - Low stock detection - SKU category visualization

RAG (Retrieval-Augmented Generation) - CSV data converted into vector
embeddings - Stored in ChromaDB - Relevant records retrieved before
answering - AI answers only from available records

KPI Dashboard - Total Inventory Count - Shipment Tracking - SKU
Coverage - AI Status Monitor

GPT Accuracy Score Each AI response is evaluated with: - Accuracy
percentage - Validation report

------------------------------------------------------------------------

SYSTEM ARCHITECTURE WORKFLOW

1.  User uploads inventory CSV
2.  Data is converted into structured documents
3.  Documents embedded using Ollama Embeddings
4.  Stored in Chroma Vector Database
5.  User asks question
6.  Retriever fetches top-k relevant records
7.  LLM generates professional response
8.  GPT Accuracy Score calculated

------------------------------------------------------------------------

TECH STACK

Frontend UI: Streamlit LLM: Ollama (gemma3:latest) Embeddings:
mxbai-embed-large Vector Database: ChromaDB Framework: LangChain Charts:
Plotly Backend: Python

------------------------------------------------------------------------

PROJECT STRUCTURE

warehouse-ai-dashboard ┣ main1.py # Streamlit AI Dashboard ┣ vector1.py
# Vector DB + CSV Ingestion ┣ vector_store/ # ChromaDB Storage ┣
README.md

------------------------------------------------------------------------

INSTALLATION GUIDE

1.  Clone Repository git clone
    https://github.com/your-username/warehouse-ai-dashboard.git cd
    warehouse-ai-dashboard

2.  Install Dependencies pip install -r requirements.txt

Required libraries: - streamlit - langchain - langchain-ollama -
langchain-chroma - chromadb - pandas - plotly

3.  Install & Run Ollama Download from: https://ollama.com

Pull required models: ollama pull gemma3 ollama pull mxbai-embed-large

4.  Ingest Inventory Data (One-Time) Edit CSV path inside vector1.py
    python vector1.py

5.  Run the Application streamlit run main1.py

Open in browser: http://localhost:8501

------------------------------------------------------------------------

HOW RAG PREVENTS HALLUCINATION - No external knowledge - No guessing -
Only retrieved inventory records - Professional structured answers -
“Data not available” if missing

------------------------------------------------------------------------

EXAMPLE USE CASES - Which products are below reorder level? - Show
inventory for Category Electronics - List shipments from Warehouse A -
Which SKU has lowest quantity? - Give supplier-wise distribution

------------------------------------------------------------------------

ACCURACY EVALUATION LOGIC - Compares response length & relevance -
Assigns score (0–100%) - Generates validation report

------------------------------------------------------------------------

FUTURE ENHANCEMENTS - Real-time IoT warehouse integration - Predictive
restocking using ML - Role-based authentication - Export AI reports as
PDF - Advanced analytics dashboard - Cloud deployment (AWS/Azure)

------------------------------------------------------------------------

WHY THIS PROJECT IS UNIQUE - Fully Local LLM (No OpenAI API needed) -
RAG-based secure answering - Animated enterprise-grade UI - AI Accuracy
reporting - Production-ready architecture

------------------------------------------------------------------------

Author: Alangara Meervin License: MIT License
