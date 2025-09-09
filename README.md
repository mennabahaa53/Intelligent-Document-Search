# 📘 Intelligent Document Search

An interactive **Question-Answering app** that lets you upload any document (PDF, DOCX, TXT) and ask natural language questions.  
The system extracts text, chunks it, builds embeddings, stores them in a **FAISS vector index**, and retrieves relevant context to generate answers using **Hugging Face Transformers**.

---

## 🚀 Features
- 📂 Upload **PDF**, **Word (DOCX)**, or **TXT** documents  
- 🔎 Semantic search with **SentenceTransformers**  
- ⚡ Fast retrieval using **FAISS vector database**  
- 🤖 Answer generation with **Flan-T5** (Hugging Face Transformers)  
- 🖥️ Simple and interactive **Gradio web UI**  

---

## 🛠️ Tech Stack
- **Python**  
- **pdfplumber** → PDF text extraction  
- **python-docx** → Word text extraction  
- **SentenceTransformers** → Embeddings  
- **FAISS** → Vector similarity search  
- **Transformers** → Flan-T5 for Q&A  
- **Gradio** → Web interface  

---

## ⚙️ How It Works
1. Extract text from the uploaded document  
2. Split text into smaller **chunks**  
3. Generate embeddings for chunks with `all-MiniLM-L6-v2`  
4. Store embeddings in a **FAISS index**  
5. For each user question:  
   - Encode the query  
   - Retrieve top-k relevant chunks  
   - Generate an answer with **Flan-T5**  

