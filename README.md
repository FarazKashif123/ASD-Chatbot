# 🤖 ASD-Chatbot– AI-Powered Autism Support Assistant
ASD Chatbot is an AI-powered assistant designed to provide informative, empathetic, and accurate answers related to Autism Spectrum Disorder (ASD).
It is built on a Retrieval-Augmented Generation (RAG) pipeline, combining Google Gemini Flash 2.0 for response generation and FAISS for fast and efficient information retrieval.

#✨ Features

🗨️ Conversational AI – Provides insightful and personalized answers related to Autism Spectrum Disorder.

💙 Empathetic Tone – Responses are sensitive and understanding towards ASD-related queries.

📚 Contextual Knowledge Retrieval – Uses FAISS to fetch the most relevant information from a custom knowledge base.

🎨 Responsive UI – Built with Streamlit, ensuring seamless use across desktop, tablet, and mobile.

🌙 Dark Mode – User-friendly dark/light theme toggle for better accessibility.

#🛠️ Tech Stack & Dependencies

PDF Extraction: pdfplumber – Extracts text from ASD-related PDFs.

Text Processing & Chunking: langchain, tqdm – Splits long text into manageable chunks.

Embeddings: sentence-transformers, numpy – Converts text into vector embeddings.

Vector Search: faiss-cpu – Enables similarity-based search.

LLM Integration: google-generativeai – Connects with Gemini Flash 2.0.

Frontend: streamlit – Interactive and simple web interface.

Environment Management: python-dotenv – Handles API keys securely.

#⚙️ How It Works
1. Knowledge Extraction

Extracts text from ASD-related PDF files using pdfplumber.

Splits large texts into smaller passages via LangChain’s RecursiveCharacterTextSplitter.

2. Embedding & Indexing

Converts passages into embeddings with SentenceTransformers.

Stores and indexes them in FAISS for efficient retrieval.

3. Context Retrieval & Response Generation

On every query, retrieves top-matching text chunks from FAISS.

Passes them to Google Gemini Flash 2.0, which generates accurate and empathetic answers.
