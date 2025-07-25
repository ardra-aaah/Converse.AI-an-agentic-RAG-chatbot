# Convex-AI - Agentic-RAG-chatbot


[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MCP](https://img.shields.io/badge/MCP-Enabled-purple.svg)](https://github.com/modelcontextprotocol)

An intelligent multi-agent RAG (Retrieval-Augmented Generation) chatbot that processes multiple document formats using Model Context Protocol (MCP) for seamless agent communication.

## 🌟 Features

- **Multi-Format Document Support**: PDF, PPTX, CSV, DOCX, TXT, Markdown
- **Agentic Architecture**: 3+ specialized agents with MCP communication
- **Semantic Search**: Advanced vector embeddings with FAISS/Chroma
- **Modern UI**: React-based interface with real-time chat
- **Multi-turn Conversations**: Context-aware dialogue system
- **Source Attribution**: View document sources for each response

## 🏗️ Architecture

```mermaid
graph TD
    A[User Interface] --> B[Coordinator Agent]
    B --> C[Ingestion Agent]
    B --> D[Retrieval Agent] 
    B --> E[LLM Response Agent]
    C --> F[Vector Store]
    D --> F
    E --> G[Language Model]
