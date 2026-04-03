📌 Conversational RAG Chatbot with LangChain

🚀 Overview

This project demonstrates a Conversational Retrieval-Augmented Generation (RAG) chatbot built using LangChain and Groq LLM.

The chatbot is capable of:

- Answering questions from a web page
- Maintaining conversation context across multiple queries
- Improving follow-up question understanding using a history-aware retriever

---

🧠 Key Concepts Implemented

- Retrieval-Augmented Generation (RAG)
- Vector Embeddings (HuggingFace MiniLM)
- Chroma Vector Database
- Web Data Ingestion using WebBaseLoader
- Context-aware conversation using chat history
- History-aware retriever for better follow-up responses

---

⚙️ Tech Stack

- Python
- LangChain
- Groq (LLaMA 3 model)
- HuggingFace Embeddings
- ChromaDB
- BeautifulSoup (for web scraping)

---

🔄 How It Works

1. Load data from a webpage using "WebBaseLoader"
2. Split text into chunks using "RecursiveCharacterTextSplitter"
3. Convert text into embeddings using HuggingFace
4. Store embeddings in Chroma vector database
5. Retrieve relevant chunks based on user query
6. Generate answer using Groq LLM
7. Maintain conversation using chat history
8. Improve follow-up queries using a history-aware retriever

---

💬 Example

Q: What is self-reflection?
A: Self-reflection is a process that allows systems or individuals to analyze past actions and improve future decisions.

Follow-up: How do we achieve it?
👉 The model uses previous context to answer correctly.

---

▶️ Installation

pip install -r requirements.txt

Create a ".env" file:

GROQ_API_KEY=your_api_key
HF_TOKEN=your_token

Run the notebook:

jupyter notebook

---

⚠️ Limitations

- Chat history is stored in memory (not persistent)
- Works on a single web source
- No user interface (CLI/Notebook only)

---

🚀 Future Improvements

- Add persistent memory (database)
- Build UI using Streamlit
- Support multiple documents
- Deploy as a web application

---

📂 Project Structure

.
├── conversationqa.ipynb
├── requirements.txt
├── .env (ignored)
└── README.md

---

📌 Notes

This project is intended for learning and understanding how conversational RAG systems work using modern LLM tools.

---
