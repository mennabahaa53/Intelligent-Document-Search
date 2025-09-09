# Intelligent-Document-Search

# 📘 Chat with Your Document

An interactive Question-Answering app that lets you upload any document (PDF, DOCX, TXT) and ask natural language questions. The system extracts text, chunks it, builds embeddings, stores them in a FAISS vector index, and retrieves relevant context to generate answers using Hugging Face Transformers.
--------------------------------------------------------------------------

🚀 Features

📂 Upload PDF, Word (DOCX), or TXT documents

🔎 Semantic search with SentenceTransformers

⚡ Fast retrieval using FAISS vector database

🤖 Answer generation with Flan-T5 (Hugging Face Transformers)

🖥️ Simple and interactive Gradio web UI

----------------------------------------------------------------------

🛠️ Tech Stack

Python

pdfplumber
 (PDF text extraction)

python-docx
 (Word text extraction)

SentenceTransformers
 (embeddings)

FAISS
 (vector similarity search)

Transformers
 (Flan-T5 for Q&A)

Gradio
 (user interface)
