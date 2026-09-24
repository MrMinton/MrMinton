# 💫 About Me:
I am a Data Science undergraduate at Multimedia University (MMU) moving from classical machine learning into **AI engineering**. I'm currently interning as an AI engineer, building LLM-powered tools that go from prototype to real users.

I love diving into datasets to solve interesting quantitative problems, whether it's modeling tournament bracket simulations or exploring complex user-behavior patterns, and I'm now applying that curiosity to building reliable, production-minded AI systems.

---

# 🚀 What I'm Working On:

- **3-Way Matching (Invoice ↔ Delivery Order ↔ Purchase Order):** An end-to-end procurement reconciliation pipeline. Supplier Invoice and Delivery Order PDFs are extracted independently with prompt-based LLM extraction (Gemini on Vertex AI, schema-driven with per-supplier prompt profiles), synced from Google Drive into a central Google Sheet. Each line is then matched against the buyer's Purchase Order by embedding similarity (Gemini/Vertex embeddings), and verified matches are reconciled quantity-by-quantity across Invoice/DO/PO into a review-ready `Reconcile` tab — surfacing mismatches like over-billing or missing deliveries automatically. Human-in-the-loop review happens directly in Sheets via an Apps Script trigger, no separate UI to maintain.
- **Project Guardrail (RAG):** A hybrid-search agent that turns a plain-language site task ("lifting works near excavation") into cited safety precautions pulled from ~600 past inspection observations — and stays silent on gibberish input. Combines pgvector similarity with Postgres full-text/trigram search via Reciprocal Rank Fusion, boosted by engineer-authored knowledge rules (task pattern → hazard category, matched by embedding similarity) and site-location matching, then filtered through a Gemini relevance pass before generating write-ups with linked inspection/rectification photos from cloud storage. Backed by Postgres/pgvector on Cloud SQL, served via FastAPI + Streamlit on Cloud Run, and iterated on real user feedback — most recently an AI-advisory, human-confirmed relevance check on retrieved photos.
- **Data Science & AI Club (DATAI):** Leading the branding and social media team.

---

# 💻 Tech Stack & Tools:

### ⚙️ Programming Languages
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### 🤖 AI Engineering
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white) ![Vertex AI](https://img.shields.io/badge/Vertex%20AI-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white) ![Hybrid Search](https://img.shields.io/badge/Hybrid%20Search-6366F1?style=for-the-badge)

**Focus areas:** retrieval-augmented generation (RAG), hybrid (vector + keyword) search relevance tuning, prompt-based document extraction, LLM pipelines, iterating on real user feedback

### ☁️ Cloud & Data Infrastructure
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Cloud Run](https://img.shields.io/badge/Cloud%20Run-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Cloud SQL](https://img.shields.io/badge/Cloud%20SQL-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-316192?style=for-the-badge&logoColor=white) ![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white) ![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)

### 📊 Data Analytics & Machine Learning
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white)

### 🌐 Frameworks & Document Formatting
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![LaTeX](https://img.shields.io/badge/latex-%23008080.svg?style=for-the-badge&logo=latex&logoColor=white)

### 🎨 Creative & Design Tools
![Adobe Premiere Pro](https://img.shields.io/badge/Adobe%20Premiere%20Pro-9999FF.svg?style=for-the-badge&logo=Adobe%20Premiere%20Pro&logoColor=white) ![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)

---

# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api/top-langs/?username=MrMinton&theme=gotham&hide_border=true&include_all_commits=false&count_private=false&layout=compact)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

---
[![](https://komarev.com/ghpvc/?username=MrMinton&icon=0&color=1)](https://visitcount.itsvg.in)
