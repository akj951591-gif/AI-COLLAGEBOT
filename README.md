# 🎓 Campus Compass – AI Chatbot

Campus Compass is an AI-powered chatbot that answers all college-related queries using official documents — not guesses.

## 🚀 Features
- Ingest PDFs, DOCX, or TXT documents.
- Store information in a semantic vector database.
- Use a RAG (Retrieval-Augmented Generation) model to provide **trustworthy**, cited answers.
- Scalable and deployable with Docker.

## 🧩 How It Works
1. Upload official campus documents (`/upload`).
2. Ask any question (`/ask?question=...`).
3. Get precise, cited answers from the documents.

## 🛠 Setup
```bash
pip install -r requirements.txt
export OPENAI_API_KEY="your_api_key"
uvicorn app:app --reload
```

Then open [http://localhost:8000/docs](http://localhost:8000/docs) for an API playground.

## 🐳 Docker
```bash
docker build -t campus-compass .
docker run -p 8000:8000 campus-compass
```

## 🧠 Example Query
**Upload:** `Student_Handbook_2025.pdf`  
**Ask:** `What's the last date to drop a course?`

**Response:**  
> "According to the Academic Calendar 2025, page 12, the last day to drop a course is 30th September."

---

🎯 *Campus Compass: Your one-stop source for verified campus information.*
    
