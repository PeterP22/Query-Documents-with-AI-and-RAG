# Advanced Document Search and Retrieval System with RAG

This GitHub repository showcases a cutting-edge document search and retrieval system leveraging Retrieval-Augmented Generation (RAG), developed using https://lightning.ai/. It intelligently queries and interacts with various documents, such as academic papers and legal documents.

## Project Overview

Our system demonstrates AI's power to quickly sift through extensive documents, providing precise answers to user queries, significantly benefiting professionals by saving time and enhancing productivity.

## Key Features

- **Document Loading and Splitting**: Utilizes `UnstructuredFileLoader` and `RecursiveCharacterTextSplitter` for document processing.
- **Embedding Generation**: Employs `HuggingFaceBgeEmbeddings` for dense vector representations of text.
- **Vector Search and Reranking**: Integrates `FAISS` and a `CrossEncoder` model for efficient searches and relevance.
- **Comprehensive AI Integration**: Combines `LangChainAI` for seamless operation across components.

## Detailed Workflow

### Document Loader
Load documents in various formats, utilizing `unstructured.io` integration with `Langchain` for high-quality preprocessing.

### Text Splitter
Split documents into manageable chunks using `Langchain`'s `RecursiveCharacterTextSplitter`, mimicking natural conversation breaks.

### Vector Database
Generate embeddings for each chunk with `BAAI/bge-large-en-v1.5` and store them in a vector database via `Langchain`'s `FAISS` integration.

### Retrieval and Re-Ranking
Retrieve and re-rank documents using `BAAI/bge-reranker-large` for the highest relevance.

## Retrieval Pipeline
This system allows users to query documents and receive the most relevant chunk, aiming to connect a Large Language Model (LLM) for conversational exchanges.

## Conclusion
This project offers a powerful pipeline for document retrieval, showcasing the potential of RAG in augmenting LLM-powered applications, setting the stage for AI-driven document interaction and knowledge discovery.
