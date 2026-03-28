# 📄 RAG-Based Document QnA Chatbot

An intelligent document-based chatbot built using **Retrieval-Augmented Generation (RAG)** that allows users to upload documents and ask questions based on their content.

---

## 🚀 Features

* 📂 Upload documents (PDF, TXT, DOCX, HTML, MD)
* 🔍 Automatic text extraction using **MarkItDown**
* ✂️ Text chunking with token-based splitting (**tiktoken**)
* 🧠 Context-aware answers using **LLM (Gemini/OpenAI API)**
* 🗂️ Semantic search with **ChromaDB (Vector Database)**
* 📊 Document summarization
* 💬 Interactive chatbot interface using **Streamlit**

---

## 🧠 How It Works (RAG Pipeline)

1. Upload document
2. Convert document → text
3. Generate summary
4. Split text into chunks
5. Store chunks in ChromaDB
6. User asks a question
7. Retrieve relevant chunks
8. LLM generates answer using context

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **Backend:** Python
* **LLM API:** Gemini / OpenAI
* **Vector DB:** ChromaDB
* **Text Processing:** MarkItDown, tiktoken

---

## 📁 Project Structure

```
.
├── main.py                  # Document upload + summarization UI
├── pages/
│   └── chatbot_page.py     # Chatbot interface
├── genai_services.py       # LLM calls, summarization, chunking
├── chroma_services.py      # ChromaDB ingestion & query
├── .env                    # API keys & configs
├── requirements.txt        # Dependencies
└── chroma_db/              # Vector database storage
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/rag-chatbot.git
cd rag-chatbot
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Setup environment variables (.env)

```
MODEL_API_KEY=your_api_key
MODEL_BASE_URL=your_base_url
MODEL_NAME=your_model_name
CHROMA_COLLECTION_NAME=your_collection
```

---

## ▶️ Run the Application

```bash
streamlit run main.py
```

---

## 💡 Usage

* Upload any supported document
* View extracted content and summary
* Click “Upload & Ingest” to store data
* Navigate to chatbot
* Ask questions related to your document

---

## 🎯 Key Highlights

* Implements **Retrieval-Augmented Generation (RAG)** architecture
* Reduces hallucination by grounding answers in document context
* Efficient semantic search using vector embeddings
* End-to-end pipeline from document ingestion to QnA

---

## 📌 Future Improvements

* Multi-document support
* Chat history memory
* UI enhancements
* Support for more file formats
* Deployment on cloud (AWS / GCP)

---

## 📷 Demo (Optional)

*Add screenshots or demo GIF here*

---

## 🤝 Contributing

Feel free to fork the repo and submit pull requests.

---

## 📜 License

This project is open-source and available under the MIT License.

