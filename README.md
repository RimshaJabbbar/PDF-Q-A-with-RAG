# PDF-Q-A-with-RAG
📄 RAG-based PDF Q&amp;A app with chat history, built using Streamlit, LangChain, Groq LLM, and HuggingFace embeddings. Upload PDFs, ask questions, and get context-aware answers with persistent chat sessions.

This project is an interactive Retrieval-Augmented Generation (RAG) application that allows users to upload multiple PDF documents and query them through a conversational interface.

Built with Streamlit for the frontend and LangChain for orchestration, the app leverages:

Groq LLM (gemma2-9b-it) for natural language question answering.

HuggingFace Embeddings (all-MiniLM-L6-v2) for semantic document retrieval.

ChromaDB as a vector store for efficient similarity search.

History-aware retriever to refine answers using previous chat context.

✨ Features

📤 Multi-PDF Upload – Upload one or more PDF documents for contextual querying.

🔍 RAG Pipeline – Retrieves relevant chunks from PDFs before answering.

🧠 Chat History Memory – Maintains session-based conversational context.

🔑 Groq API Integration – Securely use your own Groq API key.

⚡ Fast Embeddings – Uses HuggingFace embeddings with CPU fallback.

🖥 Streamlit UI – Clean and interactive interface for Q&A and chat history exploration.

🚀 How It Works

Upload your PDF(s).

The app loads and splits them into text chunks.

Embeddings are generated and stored in ChromaDB.

Ask any question in natural language.

The retriever finds relevant chunks, and the LLM answers using both documents + chat history.

🛠️ Tech Stack

Python 3.9+

Streamlit (frontend & UI)

LangChain (retrievers, prompts, memory, chaining)

Groq LLM API (for reasoning/answer generation)

HuggingFace Sentence Transformers (text embeddings)

ChromaDB (vector database for document retrieval)
