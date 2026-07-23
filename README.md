# Vitaliy Tei

Backend, data, and AI engineer who ships end-to-end systems — from data ingestion and ETL through API design, LLM orchestration, and automated evaluation. I like working where software has to make messy real-world information usable: city rules, market signals, exam prep, security data, APIs, and decision support. My strongest work combines backend engineering, data pipelines, and AI-assisted systems, with enough frontend/mobile skill to ship the full thing.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Vitaliy%20Tei-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vitaliy-tei-8562172b1) [![Email](https://img.shields.io/badge/Email-tei__tech%40outlook.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:tei_tech@outlook.com) [![Location](https://img.shields.io/badge/Brooklyn-NY-111827?style=flat)](#)

## Focus

- Backend APIs, rule engines, and data-driven services
- Multi-agent AI systems, orchestration, and decision pipelines
- RAG and LLM-evaluation pipelines
- ML/data pipelines for classification, preprocessing, and evaluation
- Turning fuzzy requirements into usable, testable software

## Featured Work

### [Crypto Orchestra](https://github.com/Vito-bc/crypto-orchestra) — Multi-Agent Trading System
Runs **seven** specialist Claude agents concurrently every hour (technical, macro regime, sentiment, funding/whale, risk, news, breakout); an LLM orchestrator weighs their signals and places limit orders across BTC, ETH, SOL, and ZEC — unattended, with Telegram alerts on every order, fill, and close.

- **Risk engine built to run live safely:** ATR-based stops tuned per asset, drawdown circuit breakers that cut position size at −5% and halt all trading at −12%, plus funding-rate, velocity, and BTC-correlation vetoes.
- **Validated honestly instead of curve-fitting:** a full-year signal scan (371 trades) and walk-forward testing across three market regimes — which showed only one of four assets carries a real out-of-sample edge, and reshaped what the system trades.
- Writes to an Obsidian "second brain" nightly (trade notes, agent decision logs, backtest summaries), structured to become a RAG knowledge base for the orchestrator.
- Python · Claude API · Pandas · Coinbase Advanced Trade · Streamlit · [Live Dashboard](https://crypto-orchestra-eqxebsnnbpg8tq6cnqzcro.streamlit.app/)

### [ARE Coach](https://github.com/Vito-bc/ARE-Coach) — AI Exam-Prep App + LLM Quality Pipeline
Cross-platform Flutter app for the Architect Registration Examination, backed by an LLM quality pipeline.

- **LLM-evaluation pipeline** that audited the app's 1,100-question bank across five quality dimensions (judgment vs. recall, distractor plausibility, answer–explanation consistency, answer leakage, embedding-based duplicates) — full audit ran under $8 via the Anthropic Batch API and produced a ranked review worklist for a licensed architect.
- **RAG generation loop:** retrieve source text, generate a grounded question, pass it through the same five-grader gate with automatic distractor repair — ~80% of generated questions survive the gate at roughly $0.07 each, with a human reviewing samples before anything ships.
- App itself: 1,100-question bank across 7 divisions, SM-2 flashcards, mock exams, and an AI Coach (chat + voice) on Firebase Cloud Functions — server-side token quotas via atomic Firestore counters, App Check, keys in Secret Manager, GitHub Actions CI.
- Flutter · Firebase · Python · Claude API · sentence-transformers · pydantic

### [ParkGuard API](https://github.com/Vito-bc/parkguard-api) — Real-Time Parking Intelligence API
REST API that runs an **ETL pipeline over NYC Open Data** and evaluates 8+ curb-side parking-rule types, returning safe / caution / blocked decisions across 4 vehicle profiles.

- Modular rules engine, in-memory TTL caching, Swagger docs, 20+ unit tests, deployed live on Render.
- Python · FastAPI · NYC Open Data · Render

### [Vulnerability Detection Pipeline](https://github.com/cunymasslab/vulnewdata) — CUNY MassLab Research
End-to-end ML pipeline (preprocessing, feature engineering, model training and evaluation) for vulnerability detection on real-world datasets, with measurable improvement over baseline. Recognized contributor on the MassLab research blog.

- Python · scikit-learn · Pandas · NumPy

## Toolbox

| Area | Tools |
| --- | --- |
| Languages | Python, SQL, Dart, JavaScript, Java, C++ |
| AI & LLM | Multi-agent orchestration, RAG, LLM evaluation, prompt engineering, Claude API, Batch API, embeddings |
| Backend & APIs | FastAPI, REST API design, async services, Firebase Cloud Functions, Firestore, pydantic |
| Data & ML | Pandas, NumPy, scikit-learn, ETL, feature engineering, backtesting, walk-forward validation |
| Mobile | Flutter (iOS · Android · Web · Desktop) |
| Delivery | Git, GitHub Actions (CI), Linux, Render, Streamlit, unit & integration testing |

## Education

**B.S. Computer Science** — Brooklyn College, CUNY (December 2025)
Dean's List (Fall 2025). Coursework: Machine Learning, Database Systems, Operating Systems, Design & Implementation of Large-Scale Applications, Data Structures.

## What I'm Building Toward

I'm focused on backend, data, and AI engineering roles where I can build reliable APIs, automate complex workflows, and ship systems that turn messy data into real decisions. I'm especially drawn to work that combines data pipelines, AI assistance, and developer-facing or decision-support systems.
