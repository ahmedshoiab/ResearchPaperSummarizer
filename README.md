# 📄 Research Paper Q&A (RAG + LLaMA-3)

An AI-powered **Research Paper Assistant** that lets you upload PDF research papers and **ask questions directly about their content**.  
It uses **Retrieval-Augmented Generation (RAG)** with **FAISS**, **Sentence Transformers**, and the **Groq LLaMA-3 API** to generate accurate, context-based answers.

---

## 🚀 Demo
<img width="1205" height="505" alt="image" src="https://github.com/user-attachments/assets/7916b906-d687-443b-bfc5-1d112782aa88" />

👉 So the pipeline is:
📄 PDF → fitz extracts → SentenceTransformer encodes → faiss stores → Groq (LLaMA-3) answers → Gradio displays.


**Flow of the app**:
1. Upload PDF →  
2. Extract text & create embeddings →  
3. Store in FAISS vector database →  
4. Retrieve top-k relevant chunks →  
5. Inject into LLaMA-3 prompt →  
6. Get contextual answers.  

---

## ✨ Features
- Upload any research paper in **PDF** format.  
- Ask natural language questions like:  
  - *"What dataset was used in this paper?"*  
  - *"What are the main contributions?"*  
- Uses **RAG pipeline** for accuracy.  
- Interactive **Gradio web app** UI.  

---

## 🛠️ Tech Stack
- **Python**  
- [SentenceTransformers](https://www.sbert.net/) – for embeddings  
- [FAISS](https://github.com/facebookresearch/faiss) – for similarity search  
- [PyMuPDF](https://pymupdf.readthedocs.io/) – for PDF text extraction  
- [Groq LLaMA-3 API](https://console.groq.com/) – for LLM responses  
- [Gradio](https://gradio.app/) – for web UI  

---

📊 Example Questions

What dataset was used in this paper?

What is the main contribution of the study?

What methods were applied for training?

Summarize the results section in simple terms.

🔮 Future Improvements

Add Summarization mode (5-bullet summaries).

Deploy to Hugging Face Spaces for free hosting.

Multi-PDF support for comparing research papers.
