<div align="center">

![](https://capsule-render.vercel.app/api?type=waving&color=0:6366F1,100:8E75B2&height=180&section=header&text=Hi,%20I'm%20Suraj&fontSize=50&fontColor=ffffff&fontAlignY=40&desc=Data%20Science%20%E2%86%92%20AI%20Engineering&descAlignY=62&descSize=20)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1200&color=8E75B2&center=true&vCenter=true&width=600&lines=Data+Science+undergrad+@+MMU;AI+engineering+intern;Building+RAG+%26+LLM+pipelines+that+real+users+rely+on)](https://git.io/typing-svg)

</div>

---

# 💫 About Me
I'm a Data Science undergraduate moving from classical machine learning into **AI engineering**. I love diving into datasets to solve quantitative problems, from tournament bracket simulations to user-behavior patterns, and I now apply that curiosity to building reliable, production-minded AI systems.

- 🎓 Data Science undergrad at Multimedia University (MMU)
- 🤖 AI engineering intern, shipping LLM-powered tools to real users
- 🎯 Focus: RAG, hybrid search, LLM document pipelines
- ☁️ Building and deploying on Google Cloud
- 🎬 Leading branding and social media for the Data Science & AI Club (DATAI)

---

# 🚀 What I'm Working On

## 🧾 3-Way Matching (Invoice ↔ Delivery Order ↔ Purchase Order)
An end-to-end procurement reconciliation pipeline that surfaces over-billing and missing deliveries automatically.

```mermaid
flowchart LR
    A["Invoice & DO PDFs<br/>(Google Drive)"] --> B["Gemini extraction<br/>schema + per-supplier prompts"]
    B --> C[("Google Sheets<br/>Invoice · DO · PO")]
    C --> D["Embedding match<br/>line items vs PO"]
    D --> E["Quantity reconciliation<br/>Invoice / DO / PO"]
    E --> F["Reconcile tab<br/>human review"]
```

- Schema-driven extraction with Gemini on Vertex AI, using per-supplier prompt profiles to handle varying document formats
- Line items matched to the buyer's Purchase Order by embedding similarity, then reconciled quantity-by-quantity
- Human-in-the-loop review happens directly in Sheets via an Apps Script trigger, so there is no separate UI to maintain

## 🦺 Project Guardrail (RAG)
A hybrid-search agent that turns a plain-language site task (e.g. "lifting works near excavation") into cited safety precautions drawn from past inspection observations.

```mermaid
flowchart LR
    Q["Site task<br/>(plain language)"] --> V["pgvector<br/>similarity search"]
    Q --> K["Postgres full-text<br/>+ trigram search"]
    V --> R["Reciprocal Rank Fusion"]
    K --> R
    R --> B["Boosts: knowledge rules<br/>+ site location"]
    B --> G["Gemini<br/>relevance filter"]
    G --> W["Cited write-up<br/>+ linked photos"]
```

- Hybrid retrieval: pgvector similarity and Postgres full-text/trigram search, fused with Reciprocal Rank Fusion
- Engineer-authored knowledge rules (task pattern → hazard category, matched by embedding similarity) and site-location matching boost relevant results
- Stays silent on gibberish input instead of returning irrelevant results
- Write-ups include linked inspection and rectification photos from cloud storage, with an AI-advisory, human-confirmed relevance check
- FastAPI + Streamlit on Cloud Run, Postgres/pgvector on Cloud SQL, iterated on real user feedback

---

# 💻 Tech Stack & Tools

### ⚙️ Programming Languages
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### 🤖 AI Engineering
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white) ![Vertex AI](https://img.shields.io/badge/Vertex%20AI-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

**Focus areas:** retrieval-augmented generation (RAG), hybrid (vector + keyword) search, prompt-based document extraction, LLM pipelines, iterating on real user feedback

### ☁️ Cloud & Data Infrastructure
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Cloud Run](https://img.shields.io/badge/Cloud%20Run-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![Cloud SQL](https://img.shields.io/badge/Cloud%20SQL-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-316192?style=for-the-badge&logoColor=white) ![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white) ![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white) ![Apps Script](https://img.shields.io/badge/Apps%20Script-4285F4?style=for-the-badge&logo=google&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)

### 📊 Data Analytics & Machine Learning
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white)

### 🌐 Frameworks & Document Formatting
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![LaTeX](https://img.shields.io/badge/latex-%23008080.svg?style=for-the-badge&logo=latex&logoColor=white)

### 🎨 Creative & Design Tools
![Adobe Premiere Pro](https://img.shields.io/badge/Adobe%20Premiere%20Pro-9999FF.svg?style=for-the-badge&logo=Adobe%20Premiere%20Pro&logoColor=white) ![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)

---

# 📊 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.shion.dev/api/?username=MrMinton&theme=gotham&hide_border=true&show_icons=true&count_private=false" />
  <img height="170" src="https://github-readme-stats.shion.dev/api/top-langs/?username=MrMinton&theme=gotham&hide_border=true&include_all_commits=false&count_private=false&layout=compact" />
</p>

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

<div align="center">

[![](https://komarev.com/ghpvc/?username=MrMinton&icon=0&color=1)](https://visitcount.itsvg.in)

![](https://capsule-render.vercel.app/api?type=waving&color=0:8E75B2,100:6366F1&height=100&section=footer)

</div>
