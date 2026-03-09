# generative-ai-project

# AI-Powered Article Search with ChromaDB + Gemini

This project demonstrates a lightweight **RAG (Retrieval-Augmented Generation)** pipeline using:

- **Chunking**: Split articles into searchable pieces  
- **LlamaIndex**: Smart chunking and preprocessing  
- **ChromaDB**: Fast vector storage and semantic search  
- **Gemini 1.5 Flash**: Accurate answers using retrieved context  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1aA6syFDGM_ME7hStWoQRb2VtgkugkJmU?usp=sharing)

---

## 🔄 Workflow

1. **Data Chunking**
   - Split full-length articles into ~100,000 chunks using LlamaIndex

2. **Embedding + Indexing**
   - Convert chunks into vectors using `all-MiniLM-L6-v2`  
   - Store in persistent ChromaDB

3. **Semantic Search**
   - Convert query to vector  
   - Retrieve top-k relevant chunks

4. **Answer Generation**
   - Combine context from results  
   - Ask Gemini 1.5 Flash for an answer

---

## 🧠 What This Project Can Do

- Process and chunk 49k+ articles into 100,000+ semantic units  
- Embed and index text into Chroma for fast search  
- Perform RAG-based Q&A using Gemini with precise retrieval  
- Easily adaptable to your own corpus  

---

## 📁 Dataset Info

- **Rows**: 49,328 articles  
- **Chunks**: 100,000+ after processing  
- **Fields**:
  - `title`: Article title  
  - `article`: Article content  



## 💡 Use Cases

- Search assistants for blogs, tutorials  
- Internal Q&A for enterprise docs  
- GenAI prototypes for educational content  
- Developer tools and codebase indexing  


Tech Stack: LlamaIndex · ChromaDB · Gemini · HuggingFace
