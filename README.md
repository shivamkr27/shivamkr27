<!-- ============ HEADER BANNER ============ -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=0:0A0A09,50:1A140B,100:0A0A09&height=180&section=header&text=Shivam%20Kumar&fontSize=55&fontColor=E0B876&fontAlignY=40&animation=fadeIn" width="100%" alt="header"/>
</div>

<!-- ============ TYPING TAGLINE ============ -->
<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=24&duration=3000&pause=800&color=C9974D&center=true&vCenter=true&width=620&lines=DevOps+%2B+Full-Stack+Developer;CS+Student+%40+UPES;I+build+cloud-native+systems;Docker+%7C+Kubernetes+%7C+CI%2FCD+%7C+Terraform;Automating+everything+that+deploys" alt="Typing SVG"/>
  </a>
</div>

<p align="center">
  <i>A DevOps-focused developer who builds full-stack apps and the cloud-native systems that ship and run them.</i>
</p>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=shivamkr27&color=c9974d&style=for-the-badge&label=Profile+Views" alt="profile views"/>
</div>

---

## 01 · About Me

- 🎓 CS student at **UPES**, specializing in **DevOps**
- ⚙️ I build **full-stack applications** and the **cloud-native infrastructure** that runs them — microservices, real-time engines, Kubernetes clusters, GitOps pipelines & AIOps tooling
- 🌱 Currently going deeper into **service mesh, platform engineering & advanced Kubernetes**
- 💬 Ask me about **Docker, Kubernetes, CI/CD, ArgoCD GitOps & Terraform**
- 📫 Reach me at **shivamkumarbxr8@gmail.com**
- ⚡ Fun fact: I once cut a deployment cycle from **30 minutes → 3** — and I'm still not satisfied

---

## 02 · Tech Stack

<p align="center"><sub>core languages, frameworks & platform tooling</sub></p>

<div align="center">
  <img src="assets/tech-marquee-core.svg" width="100%" alt="core stack marquee"/>
</div>

<p align="center"><sub>security, observability, GitOps & generative AI</sub></p>

<div align="center">
  <img src="assets/tech-marquee-devsec.svg" width="100%" alt="devsecops and AI stack marquee"/>
</div>

<p align="center"><sub>Generative AI: LangGraph agents · ChromaDB · Groq (Llama-3.3-70b)</sub></p>

---

## 03 · Featured Projects

<div align="center">

### 🧩 [gnosis-devops](https://github.com/shivamkr27/gnosis-devops) — Microservices Platform with DevOps & AIOps

[![Repo](https://img.shields.io/badge/Repository-0A0A09?style=for-the-badge&logo=github&logoColor=E0B876)](https://github.com/shivamkr27/gnosis-devops)
[![Live Demo](https://img.shields.io/badge/Live_Demo-141312?style=for-the-badge&logo=vercel&logoColor=E0B876)](http://80.225.228.31)

</div>

> Node.js · Express · React · Socket.io · PostgreSQL · Redis · Docker · Kubernetes (OKE) · Terraform · ArgoCD · GitHub Actions · Prometheus · Grafana · Gemini API

- Architected a **7-service** microservices platform (api-gateway, auth, content, progress, XP, battle, notification) with JWT auth, Helmet CSP, a relational PostgreSQL schema (8+ tables), and Redis-backed state for battle rooms & leaderboards.
- Built a **real-time multiplayer quiz battle engine** with Socket.io (1v1 + groups up to 10), live scoring & opponent-sync, on a React SPA with Zustand and Framer Motion.
- Shipped a **9-stage GitHub Actions CI/CD pipeline** — multi-arch Docker builds, Trivy CVE scanning, Cosign signing, Syft SBOMs, and ArgoCD GitOps auto-sync to OCI OKE — cutting deploys to **~3 minutes**.
- Ran the stack on **Kubernetes HPA** with PodDisruptionBudgets and hardened non-root securityContexts, observed via **Prometheus + Grafana** dashboards (per-service latency, error rates, throughput).
- Built **Kira**, an AIOps agent (Python + Streamlit + Gemini 2.5-flash) for automated cluster health scanning, anomaly detection & natural-language incident summaries.

---

<div align="center">

### 💥 [Chaos-and-DR](https://github.com/shivamkr27/Chaos-and-DR) — Chaos Engineering + Multi-Region Disaster Recovery on AWS

[![Repo](https://img.shields.io/badge/Repository-0A0A09?style=for-the-badge&logo=github&logoColor=E0B876)](https://github.com/shivamkr27/Chaos-and-DR)
[![Dashboard](https://img.shields.io/badge/Dashboard-141312?style=for-the-badge&logo=vercel&logoColor=E0B876)](https://shivamkr27.github.io/Chaos-and-DR)
[![Worker](https://img.shields.io/badge/Cloudflare_Worker-141312?style=for-the-badge&logo=cloudflare&logoColor=E0B876)](https://chaos-dr-failove.shivamkumarbxr8.workers.dev)

</div>

> Node.js · Docker · K3s · Terraform · Cloudflare Worker · Prometheus · Grafana · GitHub Actions · AWS Lambda + SNS

- Built an **active-passive multi-region system** (us-east-1 primary, us-west-2 DR) on K3s Kubernetes — Cloudflare Worker probes health per-request and fails over in **< 5 seconds** with no DNS changes.
- Ran 4 chaos experiments (pod delete, network latency injection, CPU stress, full region kill) proving **17s pod RTO**, ≥99.5% availability, and **< 5s regional failover** under real failure conditions.
- Provisioned both regions with **Terraform modules** (VPC, EC2, RDS, EIP, IAM, swap userdata) — full `terraform destroy` for zero-cost teardown between demos.
- Set up **HPA autoscaling/v2** (CPU 70% + memory 80% dual metric), Prometheus + Grafana (Node Exporter Full dashboard 1860), and AWS Lambda + SNS email alerts triggered via Cloudflare Worker on failover.
- Shipped a **GitHub Actions CI/CD pipeline** — test → multi-stage Docker build → DockerHub push (`:latest` + `:<sha>`) → `kubectl rollout` with SHA-pinned image.

---

<div align="center">

### 🔍 [Insight-engine-agent](https://github.com/shivamkr27/Insight-engine-agent) — Production-Grade Multi-Agent RAG System

[![Repo](https://img.shields.io/badge/Repository-0A0A09?style=for-the-badge&logo=github&logoColor=E0B876)](https://github.com/shivamkr27/Insight-engine-agent)
[![Live Demo](https://img.shields.io/badge/Live_Demo-141312?style=for-the-badge&logo=vercel&logoColor=E0B876)](http://80.225.212.121:8000)

</div>

> Python · LangGraph · ChromaDB · Groq (Llama-3.3-70b) · BM25 · Docker · GitHub Actions · Oracle Cloud

- Architected a **multi-agent RAG pipeline** using LangGraph — parallel agents handle sub-questions simultaneously with CRAG (Corrective RAG) loops that auto-rewrite queries on irrelevant retrievals, cutting hallucination rates significantly.
- Built a **hybrid retrieval engine** combining ChromaDB dense search + BM25 sparse search with score fusion (`0.6×dense + 0.4×BM25`) and cross-encoder reranking (`ms-marco-MiniLM-L-6-v2`) — 4 adaptive retrieval profiles auto-selected by query type (factual / conceptual / comparative / auto).
- Shipped **6 advanced modes**: Multi-Hop Reasoning (breaks complex questions into ordered search chains), Compare Mode (side-by-side document diff), Study Mode (quiz generation + auto-evaluation), Text2SQL (NL → SQLite for budget data), Web Search fallback (DuckDuckGo), and Hindi Mode (full Devanagari output).
- Implemented **LLM-as-Judge hallucination scorer** (1–5 factual grounding badge per answer), semantic **User Memory** (ChromaDB-backed, personalizes future responses), and word-by-word **token streaming** via `astream_events`.
- Deployed on **Oracle Cloud `e2.1.micro`** (1 OCPU / 1GB RAM) — ChromaDB in-process (saves ~200MB), 2GB swap for ML model loading, idle footprint of ~354MB; CI/CD via GitHub Actions (pytest → Trivy CVE scan → SSH deploy), with **163 unit tests** across all core modules.

---

## 04 · GitHub Stats

<!--
  github-readme-stats.vercel.app's public demo instance is currently paused
  (Vercel free-tier hour limit — a recurring upstream issue, not this repo).
  Restore this block once https://github-readme-stats.vercel.app/api loads again:

  <div align="center">
    <img height="165" src="https://github-readme-stats.vercel.app/api?username=shivamkr27&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&bg_color=0A0A09&title_color=E0B876&text_color=F3EFE6&icon_color=C9974D&border_color=141312" alt="stats"/>
    <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shivamkr27&layout=compact&hide_border=true&langs_count=8&bg_color=0A0A09&title_color=E0B876&text_color=F3EFE6&border_color=141312" alt="top langs"/>
  </div>
-->

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=shivamkr27&hide_border=true&background=0A0A09&ring=C9974D&fire=E0B876&currStreakLabel=E0B876&sideLabels=F3EFE6&currStreakNum=F3EFE6&sideNums=F3EFE6&dates=8F8B81&stroke=141312" alt="streak"/>
</div>

---

## 05 · Connect With Me

<div align="center">
  <a href="https://linkedin.com/in/shivamkr2004">
    <img src="https://img.shields.io/badge/LinkedIn-0A0A09?style=for-the-badge&logo=linkedin&logoColor=E0B876" alt="LinkedIn"/>
  </a>
  <a href="mailto:shivamkumarbxr8@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-0A0A09?style=for-the-badge&logo=gmail&logoColor=E0B876" alt="Gmail"/>
  </a>
  <a href="https://github.com/shivamkr27">
    <img src="https://img.shields.io/badge/GitHub-0A0A09?style=for-the-badge&logo=github&logoColor=E0B876" alt="GitHub"/>
  </a>
</div>

<!-- ============ FOOTER BANNER ============ -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=0:0A0A09,50:1A140B,100:0A0A09&height=100&section=footer" width="100%" alt="footer"/>
</div>
