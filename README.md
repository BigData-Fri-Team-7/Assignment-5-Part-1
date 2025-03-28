# Multi-Agent Research Assistant (Assignment 5.1)

An integrated research assistant that leverages three specialized agents to provide comprehensive, data-driven research reports on NVIDIA. This project combines a Snowflake Agent (for structured financial valuation data), a Pinecone-powered RAG Agent (for historical NVIDIA reports), and a Web Search Agent (for real-time insights) into one cohesive system orchestrated with LangGraph.

#Application URL:http://34.28.77.168:8501/
#Backend URL:http://34.28.77.168:8000/

## Overview

This project builds on our previous work (Assignment 4.2) to create an agentic multi-agent system that:
- **Snowflake Agent:** Connects to a Snowflake database to query structured valuation metrics sourced from Yahoo Finance.
- **RAG Agent:** Uses Pinecone to perform metadata-filtered retrieval from NVIDIA quarterly reports and generates context-aware responses.
- **Web Search Agent:** Fetches real-time industry insights using web search APIs (e.g., SerpAPI, Tavily, or Bing).

The integrated system produces research reports that include historical performance summaries, structured financial visuals, and up-to-date industry trends.

## Features

- **Multi-Agent Orchestration:** Coordinated responses from three specialized agents.
- **Hybrid Search:** Utilize Pinecone with structured metadata (Year & Quarter) for fine-tuned retrieval.
- **Real-Time Insights:** Leverage web search APIs to supplement reports with the latest news.
- **User-Friendly Interface:** Streamlit UI with FastAPI backend for research question input and filtering.
- **Dockerized Deployment:** Ready for cloud deployment with a streamlined Docker setup.

##Architectural diagram
![Editor _ Mermaid Chart-2025-03-28-210931](https://github.com/user-attachments/assets/b81d7565-6e0d-4843-a28c-8e00cb9eb13e)
