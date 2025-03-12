# Agentic RAG with LangGraph: AI Blog Search

## Overview
AI Blog Search is an Agentic RAG application designed to enhance information retrieval from AI-related blog posts. This system leverages LangChain, LangGraph, and Google's Gemini model to fetch, process, and analyze blog content, providing users with accurate and contextually relevant answers.

## LangGraph Workflow
![LangGraph-Workflow](https://github.com/user-attachments/assets/07d8a6b5-f1ef-4b7e-b47a-4f14a192bd8a)

## Demo
https://github.com/user-attachments/assets/cee07380-d3dc-45f4-ad26-7d944ba9c32b

## Features
- **Document Retrieval:** Uses Qdrant as a vector database to store and retrieve blog content based on embeddings.
- **Agentic Query Processing:** Uses an AI-powered agent to determine whether a query should be rewritten, answered, or require more retrieval.
- **Relevance Assessment:** Implements an automated relevance grading system using Google's Gemini model.
- **Query Refinement:** Enhances poorly structured queries for better retrieval results.
- **Streamlit UI:** Provides a user-friendly interface for entering blog URLs, queries and retrieving insightful responses.
- **Graph-Based Workflow:** Implements a structured state graph using LangGraph for efficient decision-making.

## Technologies Used
- **Programming Language**: [Python 3.10+](https://www.python.org/downloads/release/python-31011/)
- **Framework**: [LangChain](https://www.langchain.com/) and [LangGraph](https://langchain-ai.github.io/langgraph/tutorials/introduction/)
- **Database**: [Qdrant](https://qdrant.tech/)
- **Models**:
  - Embeddings: [Google Gemini API (embedding-001)](https://ai.google.dev/gemini-api/docs/embeddings)
  - Chat: [Google Gemini API (gemini-2.0-flash)](https://ai.google.dev/gemini-api/docs/models/gemini#gemini-2.0-flash)
- **Blogs Loader**: [Langchain WebBaseLoader](https://python.langchain.com/docs/integrations/document_loaders/web_base/)
- **Document Splitter**: [RecursiveCharacterTextSplitter](https://python.langchain.com/v0.1/docs/modules/data_connection/document_transformers/recursive_text_splitter/)
- **User Interface (UI)**: [Streamlit](https://docs.streamlit.io/)

