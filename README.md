
  <h1 align="center">👋 Hi, I'm Sri Charan Byreddy</h1>
  <h3 align="center">Full-Stack & AI Engineer · Cloud-Native · ML-Driven Systems</h3>

  <p align="center">
    <a href="mailto:charanbyreddy2717@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-charanbyreddy2717%40gmail.com-D14836?logo=gmail&labelColor=555"/></a>
    <a href="https://www.linkedin.com/in/sri-charan-byreddy/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&labelColor=555"/></a>
    <a href="https://github.com/Sricharanbyreddy9"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-Sricharanbyreddy9-181717?logo=github&labelColor=555"/></a>
    <a href="https://sricharanbyreddy.online"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-sricharanbyreddy.online-4CAF50?logo=vercel&labelColor=555"/></a>
  </p>

<p align="center">
  🚀 <strong>Code that scales, learns & ships</strong>
</p>
<p align="center">
  <code>Java / Spring Boot</code> •
  <code>Python / FastAPI</code> •
  <code>React / Vue</code> •
  <code>PostgreSQL / Supabase</code> •
  <code>Docker / AWS</code> •
  <code>RAG & Classical CV</code>
</p>

ask_me_about: |-
  - REST/GraphQL API design, event-driven patterns, CI/CD hardening
  - RAG architectures, FAISS/pgvector, embedding pipelines
  - PostgreSQL data modeling, indexing, and query plans

contact_md: |-
  - 📧 Email: <a href="mailto:charanbyreddy2717@gmail.com">charanbyreddy2717@gmail.com</a>
  - 💼 LinkedIn: <a href="https://www.linkedin.com/in/sri-charan-byreddy/">sri-charan-byreddy</a>
  - 🌐 Portfolio: <a href="https://sricharanbyreddy.online">sricharanbyreddy.online</a>
  - 🧑‍💻 GitHub: <a href="https://github.com/Sricharanbyreddy9">Sricharanbyreddy9</a>

  ## 🧰 Tech Toolbox
  | Domain | Tools |
  |---|---|
  | Languages | Python · Java · TypeScript/JavaScript · SQL · C++ |
  | Backend | Spring Boot · FastAPI · Flask · Node.js (Express) · REST · Microservices |
  | Frontend | React · Vue · Vite · Tailwind · Zustand |
  | Data | PostgreSQL · Supabase · MongoDB · Redis · SQL indexing & tuning |
  | Cloud/DevOps | Docker · GitHub Actions · Jenkins · AWS EC2/Lambda/CloudWatch |
  | ML/IR | scikit-learn · PyTorch · FAISS · SentenceTransformers · classical CV (HOG/SVM) |
  | QA/Tools | PyTest · Postman · Power BI · QGIS |

projects:
  - name: "LoanSentinel — AI Loan Risk Prediction & Monitoring"
    summary: "ML + NLP scoring with dashboards; end-to-end data flow and analytics."
    repo: "https://github.com/Sricharanbyreddy9/LoanSentinel"
    stack: ["FastAPI","Node.js (Express)","Vue (Vite)","Supabase (PostgreSQL)","Docker"]
    ports: "8000 (ML) · 5050 (Node) · 5173 (UI)"
    diagram:
    ``` |-
      Vue (Vite) UI
            │  fetches KPIs & predicts
            ▼
      Node.js (Express) ── validates → persists → aggregates
            │                           ▲
            ▼                           │
      FastAPI (ML API)  ←───────────────┘
            │
      Supabase (PostgreSQL) ← full prediction logs + NLP flags
    ```
    bullets: |-
      - ML API (FastAPI): prediction and text-risk endpoints
      - Node API (Express): validation, orchestration, DB writes/reads
      - Dashboard (Vue + Vite): KPIs, trends, what-if simulator
      - Storage (Supabase/PostgreSQL): analytics-ready schema

  - name: "RAGCare — Retrieval-Augmented Healthcare Assistant"
    summary: "LLM answers grounded in PDFs via FAISS + embeddings."
    repo: "https://github.com/Sricharanbyreddy9/RAGCare-Retrieval-Augmented-Healthcare-Assistant"
    stack: ["Flask","FAISS","SentenceTransformers","OpenAI (GPT-4)","Groq (LLaMA-3)"]
    pipeline: |-
      PDFs → Chunk & Embed → FAISS search → Prompt compose → LLM (OpenAI/Groq) → Answer
    bullets: |-
      - Upload/preload PDFs, semantic retrieval, grounded outputs
      - Dual LLM options, token/latency stats, dark/light UI

  - name: "DailyHarvest — Grocery Delivery App"
    summary: "React + Supabase full-stack app with clean, modern UI."
    repo: "https://github.com/Sricharanbyreddy9/DailyHarvest"
    stack: ["React","TypeScript","Tailwind","Zustand","Supabase"]
    bullets: |-
      - Auth, catalog, cart, checkout; lbs ↔ kg conversion; responsive and dark mode
      - Admin: products, inventory, orders (role-based)

  - name: "Fine-Grained Image Classification (HOG + MLP + ELLF + CNN)"
    summary: "Compare classic features vs deep ensembles for visually similar classes."
    report_or_code: "https://github.com/Sricharanbyreddy9/Advancing-Fine-Grained-Recognition-Through-Weakly-Supervised-Learning"
    models: |-
    ```
      HOG → SVM      (baseline)
      HOG → MLP      (nonlinear head)
      ELLF + CNN     (localized parts + conv features)
    ```
    bullets: |-
      - Pipelines: HOG+SVM, HOG+MLP, ELLF+CNN (weak supervision)
      - Results (sample): HOG+SVM 85%, HOG+MLP 88%, ELLF+CNN 95%

  - name: "AthleteSphere — Sports Data Intelligence (Olympics)"
    summary: "BCNF-normalized schema + indexed queries + API for BI."
    report_or_code: "https://github.com/Sricharanbyreddy9/AthleteSphere-Optimized-Sports-Analytics-DB/blob/main/Report/Report.pdf"
    stack: ["Flask","PostgreSQL","SQL tuning","Power BI"]
    flow: |-
      REST API → Postgres (BCNF) → Indexed joins → Power BI dashboards
    bullets: |-
      - Entities: athletes, teams, events, medals; composite FKs; tuned indexes
      - Longitudinal and demographic queries under ~150 ms on 10K+ rows

quick_start_block: |-
  ML API:
    cd services/ml-api
    uvicorn main:app --reload --port 8000
  Node API:
    cd services/node-api
    npm install
    npm run dev    # http://localhost:5050
  Frontend:
    cd services/node-api/loan-risk-dashboard
    npm install
    npm run dev    # http://localhost:5173

activity_stats_html: |-
  <p align="center">
    <img src="https://github-readme-streak-stats.herokuapp.com?user=Sricharanbyreddy9&theme=tokyonight" alt="Streak" width="49%"/>
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sricharanbyreddy9&layout=compact&theme=tokyonight" alt="Top Langs" width="49%"/>
  </p>

footer_html: |-
  <sub>Tip: This is a special repository. Name it exactly <b>Sricharanbyreddy9</b> and keep it <b>Public</b> so this README shows on your profile.</sub>
