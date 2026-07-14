# PDF RAG using LangChain

This project demonstrates a basic Retrieval-Augmented Generation (RAG) pipeline using **LangChain**, **FAISS**, **Hugging Face Embeddings**, and **Ollama**. The application loads a PDF document, converts it into vector embeddings, retrieves the most relevant chunks for a user query, and generates an answer using a local Large Language Model.

## Project Objective

The objective of this project is to understand the complete RAG pipeline, including document loading, text chunking, embedding generation, vector storage, retrieval, and response generation.

## Features

* PDF document loading
* Text chunking using `RecursiveCharacterTextSplitter`
* Sentence Transformer embeddings
* FAISS vector database
* Similarity-based retrieval
* Prompt construction using retrieved context
* Local inference using Ollama

## Project Workflow

```text
PDF Document
      │
      ▼
Document Loader
      │
      ▼
Text Splitter
      │
      ▼
Embedding Model
      │
      ▼
FAISS Vector Store
      │
      ▼
Retriever
      │
      ▼
Prompt
      │
      ▼
Ollama (DeepSeek)
      │
      ▼
Answer
```

## Technologies Used

* Python
* LangChain
* Hugging Face Embeddings
* FAISS
* Ollama
* DeepSeek-R1
* PyPDFLoader

## Installation

Clone the repository

```bash
git clone <repository-url>
```

Install dependencies

```bash
pip install -r requirements.txt
```

Install and start Ollama, then pull the required model

```bash
ollama pull deepseek-r1:1.5b
```

Run the notebook or Python script.

## What I Learned

Through this project, I learned:

* Loading PDF documents
* Splitting documents into chunks
* Generating embeddings
* Creating a FAISS vector database
* Performing similarity search
* Retrieving relevant context
* Building prompts using retrieved documents
* Connecting a local LLM with a RAG pipeline

## Future Improvements

* Conversational RAG
* Hybrid Search (BM25 + Vector Search)
* Reranking
* Metadata filtering
* Streamlit interface
* LangGraph-based RAG workflow

## Project Structure

```text
├── RAG.ipynb
├── requirements.txt
├── sample.pdf
├── README.md
└── .gitignore
```
