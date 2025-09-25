# AI Data Readiness Checker (Prototype)

A prototype tool to quickly evaluate whether a dataset is **ready for ML workflows**.  
Built with **FastAPI + Python** on the backend and **React + Tailwind** on the frontend.

---

## 🚨 Problem
Teams waste hours checking if data is usable for ML. Missing values, duplicates, and schema issues often derail projects late in the pipeline.

---

## 💡 Solution
This tool runs **automated readiness checks**:
- Schema + column type detection  
- % Missing values, duplicates  
- Basic scoring across dimensions (completeness, validity, uniqueness, timeliness)  
- AI assistant (OpenAI API) to suggest improvements  

---

## 🖥️ Demo (CSV Mode)
- Upload a CSV in the frontend (drag-and-drop UI).
- View a **Data Profile** with readiness scores.  
- Ask questions in **AI Studio** (e.g., “How can I fix missing values?”).  
- Export a **Data Readiness Report** in markdown.  

---

## 🛠️ Tech Stack
- **Backend:** FastAPI, Pandas, NumPy, Pydantic:contentReference[oaicite:0]{index=0}  
- **Frontend:** React 18, Tailwind, Highlight.js:contentReference[oaicite:1]{index=1}:contentReference[oaicite:2]{index=2}  
- **Infra/Other:** Node.js + Express (Snowflake SDK planned):contentReference[oaicite:3]{index=3}  

---

## ⚡ Quickstart

### Backend
```bash

cd ai-data-readiness-checker
pip install -r requirements.txt
uvicorn server:app --reload

npm install
npm start

```

Then open: http://localhost:3000
