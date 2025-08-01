# Code Helper Bot using RAG and LangGraph

This project implements a code assistant bot capable of generating and explaining code using a Retrieval-Augmented Generation (RAG) architecture integrated with LangGraph. The system combines embeddings, vector search, and a powerful language model to deliver accurate and context-aware code assistance.

## Overview

The application supports the following capabilities:

- **Code Generation and Explanation**: Users can input code or questions to receive generated code snippets or detailed explanations.
- **Retrieval-Augmented Generation**: Relevant context is retrieved from a vector store to guide the model’s output.
- **LangGraph-Based Architecture**: Workflow orchestration and decision-making are handled through LangGraph.
- **Embeddings**: Utilizes the `BAAI/bge-large-en-v1.5` model to embed user queries and documents.
- **Vector Store**: Employs ChromaDB to store and retrieve semantically similar queries and responses.
- **Language Model**: Uses `Qwen/Qwen2.5-Coder-7B-Instruct` for high-quality code generation and explanation.
- **Evaluation**: Model performance was assessed using a subset of 10 examples from the MBPP dataset, achieving 80% accuracy while maintaining efficient GPU usage and fast inference time.
- **Deployment**: The application is deployed using Gradio's ChatBotInterface for interactive usage.

## System Architecture

A visual representation of the LangGraph application flow is provided below:

<img width="480" height="580" alt="Capture2" src="https://github.com/user-attachments/assets/763b070e-881c-4994-82da-68d13c902759" />


## Technology Stack

| Component       | Description                              |
|----------------|------------------------------------------|
| Embedding Model | `BAAI/bge-large-en-v1.5`                 |
| Vector Store    | ChromaDB                                 |
| Language Model  | `Qwen/Qwen2.5-Coder-7B-Instruct`         |
| Framework       | LangGraph                                |
| Deployment      | Gradio ChatBotInterface                  |
| Evaluation Data | MBPP (Mostly Basic Python Problems)      |

## Evaluation

- **Accuracy**: 80% on a selected sample of MBPP tasks  
- **Performance Considerations**: Designed for efficient GPU utilization and optimized inference speed
