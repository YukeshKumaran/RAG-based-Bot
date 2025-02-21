# 📚 ChatPDF Bot – AI-Powered PDF Q&A  

This project is an **interactive AI chatbot** that allows users to **upload PDF documents** and ask **questions** about their content. It uses **Google Gemini AI** and **FAISS vector storage** for **Retrieval-Augmented Generation (RAG)**.  

## 🚀 Features  
✅ **Upload multiple PDFs** and extract text  
✅ **AI-powered Q&A** using document content  
✅ **Fallback to Gemini AI** for general queries  
✅ **Efficient document search** with FAISS  
✅ **Streamlit UI** for easy interaction  

## 🛠️ How It Works  
1️⃣ **Extract Text from PDFs**  
   - Uses `PyPDF2` to **read PDF content**.  
2️⃣ **Chunk & Store in FAISS**  
   - Splits text using `RecursiveCharacterTextSplitter` and **stores embeddings**.  
3️⃣ **Question Answering with AI**  
   - If the query **matches PDF content**, retrieves an answer.  
   - Otherwise, it uses **Gemini AI** for a general response.  

## 🖥️ Technologies Used  
- **Streamlit** → For UI  
- **LangChain** → For RAG-based retrieval  
- **FAISS** → Vector search database  
- **Google Gemini AI** → LLM-powered responses  

## 📂 Code Structure  
- `app.py` → Main Streamlit app  
- `get_pdf_text()` → Extracts text from PDFs  
- `get_vector_store()` → Embeds and stores text in FAISS  
- `validate_question_relevance()` → Checks if the query is related to the document  
- `user_input()` → Handles user queries and responses  

---

🔗 **Run the app using:**  
```bash
streamlit run app.py
