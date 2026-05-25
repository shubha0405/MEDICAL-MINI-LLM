# 🏥 MediAssist — AI-Powered Medical Q&A Chatbot

MediAssist is a **full-stack AI-powered medical Q&A chatbot** that leverages **Retrieval-Augmented Generation (RAG)** and a **Groq-powered Large Language Model (LLM)** to answer health-related queries using **trusted medical literature**.

The platform combines **semantic search, document retrieval, and generative AI** to provide contextual, source-backed responses in an interactive chat interface.

🔗 **Live Demo:** https://mini-medical-llm.vercel.app

---

## 🚀 Features

- 🔐 **JWT Authentication** – Secure user login and session management
- 💬 **Persistent Chat History** – Stores previous conversations for continuity
- 📚 **Retrieval-Augmented Generation (RAG)** – Fetches relevant medical knowledge before generating responses
- 🧠 **Groq-powered LLM Integration** – Fast and intelligent response generation
- 🔍 **FAISS Semantic Search** – Efficient vector similarity retrieval
- 📄 **PDF Export** – Export chat conversations as downloadable PDF reports
- 📖 **Source Citations** – Displays references from retrieved medical literature
- ⚡ **Responsive Full-Stack UI** – Smooth frontend experience with Next.js

---

## 🏗️ Architecture Workflow

User Query  
↓  
Frontend (Next.js)  
↓  
REST API Request  
↓  
FastAPI Backend  
↓  
JWT Validation  
↓  
Embedding Generation  
↓  
FAISS Vector Search  
↓  
Relevant Medical Context Retrieval  
↓  
Groq LLM Response Generation  
↓  
Response + Source Citations  
↓  
Frontend Display / PDF Export

---

## 🛠️ Tech Stack

### Frontend
- Next.js
- React
- Tailwind CSS

### Backend
- FastAPI
- Python
- REST APIs
- JWT Authentication

### AI / ML
- Retrieval-Augmented Generation (RAG)
- Groq LLM
- Sentence Transformers / Embeddings
- FAISS Vector Database

### Database
- MongoDB

### Deployment
- Vercel (Frontend)
- Backend API Hosting

---

## 📂 Project Structure

```bash
MediAssist/
│── frontend/          # Next.js frontend
│── backend/           # FastAPI backend
│── routes/            # API routes
│── models/            # Database schemas
│── auth/              # JWT authentication logic
│── retriever/         # FAISS retrieval pipeline
│── generator/         # LLM response generation
│── utils/             # Helper functions
│── requirements.txt
│── README.md
```

---

## ⚙️ How It Works

1. User enters a medical question
2. Query is sent from frontend to backend via REST API
3. Backend validates user authentication
4. Query is converted into vector embeddings
5. FAISS retrieves semantically relevant medical documents
6. Retrieved context is passed to Groq-powered LLM
7. LLM generates contextual response
8. Sources are cited and returned to frontend
9. Chat history is stored in MongoDB
10. User can export conversation as PDF

---

## 🔧 Installation & Setup

### Clone Repository

```bash
git clone https://github.com/yourusername/mediassist.git
cd mediassist
```

### Backend Setup

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🔐 Environment Variables

Create a `.env` file in backend:

```env
GROQ_API_KEY=your_api_key
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
```

---

## 🎯 Future Improvements

- Voice-based medical assistant
- Multi-language support
- Medical image analysis integration
- Appointment booking integration
- Fine-tuned domain-specific medical model

---

## ⚠️ Disclaimer

MediAssist is intended for **educational and informational purposes only** and should **not replace professional medical advice, diagnosis, or treatment**.

---

## 👩‍💻 Author

**Shubha A**  
Engineering Student | AI & Full-Stack Developer

---

## ⭐ Show Your Support

If you found this project useful, consider giving it a **star ⭐ on GitHub**.
