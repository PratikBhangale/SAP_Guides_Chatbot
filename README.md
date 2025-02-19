# SAP Installation Guides Search Automation Using Agentic AI and Multi-Modal RAG

This project automates the search and retrieval of SAP installation guides by leveraging cutting-edge AI and retrieval techniques. It integrates an interactive conversational interface with advanced document embedding and vector search, streamlining user queries and improving documentation accessibility.

## Overview

The project comprises two main components:

- **Chat With Llama:** An interactive chat interface built with Streamlit that uses the Ollama Llama 3.1 model via LangChain for natural language processing. This component handles user queries by retrieving context from previous interactions and providing real-time responses. :contentReference[oaicite:0]{index=0}

- **Data Stores:** A module that processes and embeds uploaded PDF documents (SAP installation guides) using LangChain's FAISS vector store and Ollama embeddings. The module splits documents into manageable chunks and creates a searchable database to support efficient and accurate retrieval. :contentReference[oaicite:1]{index=1}

## Features

- **Agentic AI Chat Interface:** 
  - Uses Ollama's Llama 3.1 for generating responses.
  - Maintains chat history for improved context and user experience.
  - Built with Streamlit for an intuitive web interface.

- **Multi-Modal Retrieval-Augmented Generation (RAG):**
  - Converts PDF documents into vector embeddings.
  - Utilizes LangChain's FAISS for fast similarity search.
  - Integrates document splitting and embeddings using Ollama's "all-minilm" model.

- **Automated Document Embedding:**
  - Upload and process SAP installation guide PDFs.
  - Create a local vector store for efficient document retrieval.

## Technologies Used

- **Programming Language:** Python
- **Web Framework:** Streamlit
- **LLM & NLP:** Ollama (Llama 3.1) via LangChain
- **Document Processing:** PyPDFLoader, RecursiveCharacterTextSplitter
- **Vector Embeddings & Search:** OllamaEmbeddings (all-minilm), FAISS
- **Environment Management:** dotenv

## Prerequisites

- Python 3.8 or higher
- [Streamlit](https://streamlit.io/)
- [Ollama](https://ollama.ai/) (installed and running)
- Required Python libraries (installable via `pip install -r requirements.txt`)

## Installation & Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/sap-search-automation.git
   cd sap-search-automation

   
2.  **Install Dependencies:**

Ensure you have Python 3.8+ installed, then run:
    ```bash
    pip install -r requirements.txt

