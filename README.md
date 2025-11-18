# RAG Agent (LangGraph + LangChain + Chroma)

📘 Project Overview

This project focuses on building a medical document question–answering AI agent using Retrieval-Augmented Generation (RAG) and LangGraph.
The system intelligently retrieves relevant medical information from a curated knowledge base and generates accurate, context-aware answers using an LLM.

Designed for reliability and clarity, the agent simulates a multi-step reasoning process with Planning → Retrieval → Answer Generation → Reflection, ensuring better quality responses for medical queries.

This project serves as an advanced healthcare AI assistant that supports medical learning, research, clinical insights, and evidence-based decision-making.

🧩 Modules & Sub-Modules
1. 🏠 Home

Project introduction

Workflow overview

Quick navigation to agent functionalities

2. ❓ Medical Q&A Agent
Query Input

Users ask free-form medical questions

Example: “What are symptoms of hypertension?”

RAG-Based Retrieval

Retrieves relevant medical context from vector database (ChromaDB)

Uses embeddings to match information from medical documents

Answer Generation

LLM generates a medically accurate answer using retrieved context

Reflection Step

Validates answer relevance

Checks if the response addresses the question

Produces a confidence/reflection output

3. 📚 Medical Knowledge Base

Upload multiple medical PDFs or text files

Automatic text chunking

Embedding generation (OpenAI / HuggingFace)

Indexed & stored in ChromaDB

4. 📊 Agent Pipeline Dashboard

Shows each stage of the agent run

Logs pipeline output:

🧠 Plan

🔍 Retrieve

✍️ Answer

🔁 Reflect

Useful for debugging and explainability

5. 👥 About Us
Our Team

Contributors & developer info

Our Mission

Make medical information retrieval accessible, safe, and efficient

Demonstrate modern LLM-based RAG pipeline using LangGraph

6. 🆘 Help
Support

How to run the project

How to load medical documents

Troubleshooting steps

FAQ

Common questions about RAG, LangGraph, embeddings, etc.

⚙️ Tech Stack
Backend / AI Frameworks

LangGraph (agent workflow)

LangChain / LlamaIndex (RAG pipeline)

ChromaDB (vector storage)

OpenAI / HuggingFace Embeddings

Python

Optional Frontend

Streamlit or Gradio (interactive UI)

Models

LLMs: OpenAI GPT, HuggingFace models

Embeddings: text-embedding-3-small / all-mpnet-base-v2

Database

ChromaDB (Vector DB)

SQLite (metadata storage)

## Quickstart

1. Create a virtual env and install requirements:
   ```bash
   pip install -r requirements.txt
   ```

2. Put your source documents into `data/` (your uploaded PDF is already copied as `data/source.pdf`).

3. Open the notebook:
   ```bash
   jupyter lab  # or jupyter notebook
   ```

4. Run the notebook cells to:
   - Load & split documents
   - Build embeddings & Chroma store
   - Construct the LangGraph
   - Query the agent

🚀 Features

✔ Ask medical-related questions and get accurate AI-generated answers
✔ Intelligent RAG pipeline retrieves only the most relevant context
✔ Multi-step agent workflow ensures validated, high-quality outputs
✔ Supports multiple medical document formats (PDF, TXT)
✔ Vector search enhances precision of answers
✔ Simple, interactive interface (if Streamlit added)
✔ Modular design for improving or replacing models easily

🛠️ Environment Setup

Install required libraries:

langgraph

langchain

chromadb

openai

sentence-transformers

pypdf

python-dotenv

streamlit   
      

🎯 Future Work

Add evaluation metrics (RAGAS, BLEU, Rouge, LLM-as-a-Judge)

Integrate medical ontology knowledge graph

Add voice-based medical Q&A

Deploy as a secure cloud API

Add multi-modal medical support (X-rays, prescriptions)

Improve medical safety with clinical guardrails
