# Vitaliy Tei

**Backend & AI engineer** building systems that turn complex data and rules into testable decisions. My work spans Python services, AI orchestration, evaluation pipelines, and cross-platform products. I care about clear boundaries, reproducible evidence, and software that says plainly what it can do today.

[LinkedIn](https://www.linkedin.com/in/vitaliy-tei-8562172b1) · [Email](mailto:tei_tech@outlook.com) · Brooklyn, New York

## Selected work

### TEO Jarvis — AI runtime and orchestration platform
**Python · Linux namespaces · Landlock · DAG workflows · capability security** &nbsp;|&nbsp; **Private repository; active development**

Building a local-first execution foundation for AI-assisted workflows. The runtime uses default-deny policy, explicit authority, deterministic verification, and structured audit records.

- Designed bounded agent execution with declared time, tool-call, and correction limits. A validated DAG engine supports dependencies, branches selected from verified outcomes, forward recovery routes, approval gates, and bounded concurrency.
- Implemented run-bound, single-use capability authorization. Acceptance contracts and deterministic checks decide whether a step succeeds; an agent's own success claim does not.
- Isolated provider processes with Linux namespaces, a private `pivot_root` filesystem, read-only mounts, and Landlock. A mediated egress path limits an approved run to its authorized HTTPS destination, with DNS resolution, connection, and TLS SNI checks.
- Kept API credentials outside the repository, validated file ownership and permissions, delivered secrets over a dedicated file descriptor, and centralized redaction. Versioned traces record policy decisions and observed provider outcomes.
- Tested sandbox escape attempts against host files, processes, and network access in an adversarial corpus. The production runtime has no third-party Python dependencies.

The first real provider call requires a separate human approval for that run. Broader development-agent integrations and domain packs remain future work; this is an actively developed execution foundation.

### [Crypto Orchestra](https://github.com/Vito-bc/crypto-orchestra) — multi-agent trading research
**Python · Claude API · Coinbase data · reproducible research** &nbsp;|&nbsp; **Public repository; monitor mode**

Designed a seven-specialist-agent signal pipeline with a deterministic risk gate and paper-order path. The research program then tested whether a directional strategy could clear execution costs and a credible evidence threshold.

- Built walk-forward and feasibility analyses, explicit trial records, and a research verification harness that regenerates committed results from pinned inputs and dependencies.
- The evaluated directional approaches did **not** demonstrate an actionable edge. The trading pipeline is currently idle; no live orders or scheduled LLM trading are running.
- Daily execution-cost and hourly funding monitors support a future reassessment if conditions change.

The negative result is part of the work: the repository records why the system stays in paper/shadow mode instead of claiming a profitable strategy.

### ARE Coach — architecture exam-prep app
**Flutter · Firebase · Python · RAG · LLM evaluation** &nbsp;|&nbsp; **Private repository; preparing for release**

A cross-platform study product for the Architect Registration Examination. The app combines practice questions, mock exams, flashcards, study planning, and an AI-assisted study experience.

- Built a source-grounded content workflow: retrieve supporting material, generate candidate questions, evaluate answer and explanation consistency, distractor quality, leakage, and duplicates, then route content to architect review.
- Developed the Flutter/Firebase application and release infrastructure, including backend quotas, app integrity checks, automated tests, and purchase/entitlement flows.
- The source code and question bank are private while the product approaches production. I can discuss architecture, engineering decisions, and the review process without sharing proprietary content.

### [CUNY MASS Lab](https://cunymasslab.github.io/people/) — vulnerability detection research and developer tooling
**Python · scikit-learn · reproducible environments · remote debugging** &nbsp;|&nbsp; **2025 capstone research**

For my CISC 4900 capstone, worked with Professor Hui Chen's research group at Brooklyn College on machine-learning approaches to software vulnerability detection.

- Built and evaluated a Python ML pipeline for real-world vulnerability data, covering preprocessing, feature engineering, model training, and comparison with a baseline.
- Documented how new contributors can set up a reproducible Python environment and debug long-running experiments on a remote Linux cluster.
- Coauthored two guides published on the lab's website with Josemar Ochoa: [Python development environment for lab research](https://cunymasslab.github.io/blog/2025/python-environment-setup/) and [remote debugging with VS Code and DebugPy](https://cunymasslab.github.io/blog/2025/remote-debugging-vscode/).

### [ParkGuard API](https://github.com/Vito-bc/parkguard-api) — explainable parking-rule decisions
**Python · FastAPI · NYC Open Data** &nbsp;|&nbsp; **Public repository; portfolio MVP**

A REST API that combines curb rules, location data, and vehicle profiles to return a `safe`, `caution`, or `blocked` parking decision with rule-level explanations.

- Handles time-window restrictions, hydrant proximity, and vehicle-specific rules for passenger, truck, taxi, and for-hire profiles.
- Includes confidence and freshness signals, caching, API documentation, and unit/integration tests.

## Tools I use

| Area | Stack and methods |
| --- | --- |
| Backend | Python, FastAPI, REST APIs, async services, Firebase Cloud Functions, Firestore |
| AI systems | Agent orchestration, capability and approval boundaries, RAG, LLM evaluation, embeddings |
| Data and ML | Pandas, NumPy, scikit-learn, ETL, backtesting, walk-forward evaluation |
| Product | Flutter, Dart, Firebase, JavaScript |
| Engineering | SQL, Java, C++, Git, GitHub Actions, Linux, automated testing |

## Education

**B.S. Computer Science — Brooklyn College, CUNY**  
Dean's List (Fall 2025). Coursework includes machine learning, databases, operating systems, and data structures.

## Let's connect

I am interested in backend, data, and AI engineering roles where reliability and measured outcomes matter. Reach me by [email](mailto:tei_tech@outlook.com) or [LinkedIn](https://www.linkedin.com/in/vitaliy-tei-8562172b1).
