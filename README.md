<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:020617,35:0f172a,70:0e7490,100:22d3ee&height=300&section=header&text=DEVBRATH%20SINGH%20GAUTAM&fontSize=42&fontColor=F8FAFC&fontAlignY=36&desc=AI%20%2F%20ML%20Intern%20%20%E2%80%A2%20%20RAG%20%20%E2%80%A2%20%20FastAPI%20%20%E2%80%A2%20%20TypeScript&descAlignY=56&descSize=17&animation=fadeIn" width="100%" alt="header"/>
</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=22D3EE&center=true&vCenter=true&width=820&lines=Building+systems+that+retrieve%2C+verify%2C+and+ship;Query+%E2%86%92+agent+%E2%86%92+evidence+%E2%86%92+DeBERTa+%E2%86%92+refuse+or+answer;Data+%E2%86%92+leak-safe+features+%E2%86%92+P10%2FP50%2FP90+%E2%86%92+API+%E2%86%92+UI;How+I+learn%3A+break+it%2C+measure+it%2C+serve+it)](https://github.com/devcodes007)

</div>

<div align="center">

<a href="https://github.com/devcodes007"><img src="https://img.shields.io/badge/GitHub-devcodes007-020617?style=for-the-badge&logo=github&logoColor=67e8f9" alt="GitHub"/></a>
<a href="https://www.linkedin.com/in/devbrath-singh-gautam-50951029a/"><img src="https://img.shields.io/badge/LinkedIn-Connect-020617?style=for-the-badge&logo=linkedin&logoColor=38bdf8" alt="LinkedIn"/></a>
<a href="mailto:devgautam030@gmail.com"><img src="https://img.shields.io/badge/Email-devgautam030-020617?style=for-the-badge&logo=gmail&logoColor=22d3ee" alt="Email"/></a>
<a href="https://docuverify-six.vercel.app"><img src="https://img.shields.io/badge/Live-DocuVerify-020617?style=for-the-badge&logo=vercel&logoColor=22d3ee" alt="DocuVerify"/></a>
<a href="https://frontend-livid-seven-76.vercel.app"><img src="https://img.shields.io/badge/Live-Forecasting-020617?style=for-the-badge&logo=react&logoColor=22d3ee" alt="Forecasting"/></a>

</div>

<br/>

```text
role        →  AI / ML intern
education   →  B.Tech ECE (IoT) · NSUT · 2027
now         →  DRDO · Scientific Analysis Group
loop        →  data → model → validate → FastAPI → TypeScript UI
```

I do not stop at a trained model. I design the system around it — retrieval, leakage checks, APIs, and a UI — so the miss is visible instead of hidden.

---

<div align="center">

## featured work

</div>

<table>
<tr>
<td width="50%" valign="top">

### [DocuVerify](https://github.com/devcodes007/Docuverify_2) — Agentic RAG

[![Live](https://img.shields.io/badge/live_demo-docuverify-22d3ee?style=flat-square)](https://docuverify-six.vercel.app)
[![Repo](https://img.shields.io/badge/github-Docuverify__2-0ea5e9?style=flat-square&logo=github)](https://github.com/devcodes007/Docuverify_2)

Agent routes lookup / comparison / multi-hop, hybrid BM25 + dense retrieval, up to 3 retries. Fine-tuned **DeBERTa-v3-small** labels `SUPPORTED` / `CONTRADICTED` / `UNSUPPORTED` — a second model, not another LLM prompt. Unsupported answers are refused.

FastAPI backend (ingest, query, SSE traces) + TypeScript frontend.

`RAG` `FastAPI` `TypeScript` `ChromaDB` `DeBERTa` `BM25`

</td>
<td width="50%" valign="top">

### [State Demand Forecasting](https://github.com/devcodes007/State-Electricity-Demand-Forecasting-) — P10/P50/P90

[![Live](https://img.shields.io/badge/live_demo-forecasting-22d3ee?style=flat-square)](https://frontend-livid-seven-76.vercel.app)
[![Repo](https://img.shields.io/badge/github-demand_forecasting-0ea5e9?style=flat-square&logo=github)](https://github.com/devcodes007/State-Electricity-Demand-Forecasting-)

LightGBM quantile regression for Delhi, Gujarat, Karnataka on 10k+ days. Leakage-safe lags, chronological splits, validation-only `α = 0.25` (P50 pinball **3.48**, **51.8%** coverage). Gujarat shift and ~12% crossing stay in the dashboard.

FastAPI backend + TypeScript / React client.

`Python` `LightGBM` `FastAPI` `TypeScript` `React` `Pandas`

</td>
</tr>
</table>

---

<div align="center">

## how I learn

</div>

I do not collect tutorials. I pick a failure I can measure, then force it through a full loop until a UI can show the miss.

```mermaid
flowchart LR
  A["1 · Find the break"] --> B["2 · Draw the pipeline"]
  B --> C["3 · Smallest honest experiment"]
  C --> D["4 · Metric that can prove me wrong"]
  D --> E["5 · FastAPI + types"]
  E --> F["6 · TypeScript UI"]
  F --> A

  style A fill:#0f172a,stroke:#22d3ee,color:#e2e8f0
  style B fill:#0f172a,stroke:#38bdf8,color:#e2e8f0
  style C fill:#0f172a,stroke:#2dd4bf,color:#e2e8f0
  style D fill:#0f172a,stroke:#34d399,color:#e2e8f0
  style E fill:#0f172a,stroke:#a78bfa,color:#e2e8f0
  style F fill:#0f172a,stroke:#f472b6,color:#e2e8f0
```

| step | what I actually do |
| :--- | :--- |
| **Find the break** | Hallucinated RAG answer. Leaky lag. Gujarat regime shift. Crossing quantiles. |
| **Draw the pipeline** | Paper / docs until I can sketch boxes: data → model → check → API → UI. |
| **Smallest honest experiment** | Document-level splits. Causal `shift(1)`. Validation-only `α`. Bounded retries. |
| **Metric that can prove me wrong** | Groundedness label, pinball, coverage, crossing — not “it looked good.” |
| **Serve it** | FastAPI schemas, REST, SSE traces, errors instead of invented history. |
| **Show it** | TypeScript client so a human sees refuse / shift / crossing. |

`problem → experiment → eval → backend → UI → what still fails`

---

<div align="center">

## system architecture

how both products are the same machine

</div>

```mermaid
flowchart TB
  subgraph IN["WORLD"]
    PDF["PDFs / docs"]
    TS["Daily demand · weather · holidays"]
  end

  subgraph PREP["PREPARE — never cheat the split"]
    CHUNK["Structure-aware chunking<br/>document_id stays with every example"]
    FEAT["State-grouped causal lags<br/>shift 1 · rolling · EWMA α on val only"]
  end

  subgraph STORE["INDEX / MODEL"]
    BM25["BM25 · identifier tokenizer"]
    DENSE["Dense embeddings · Chroma"]
    LGBM["LightGBM P10 / P50 / P90"]
  end

  subgraph THINK["DECIDE"]
    ROUTER["Query router<br/>LOOKUP · COMPARISON · MULTI-HOP"]
    RETRY["Hybrid retrieve<br/>evidence gap → reformulate ≤ 3"]
    GEN["Evidence-only generation<br/>citations"]
    QPRED["Quantile inference<br/>one-step, same features as train"]
  end

  subgraph CHECK["VERIFY — second opinion"]
    DEB["DeBERTa-v3-small<br/>SUPPORTED / CONTRADICTED / UNSUPPORTED"]
    MET["Pinball · coverage · crossing<br/>Gujarat train vs val shift"]
  end

  subgraph SERVE["SHIP"]
    API["FastAPI REST + SSE"]
    UI["TypeScript / React"]
  end

  PDF --> CHUNK --> BM25
  CHUNK --> DENSE
  TS --> FEAT --> LGBM

  BM25 --> ROUTER
  DENSE --> ROUTER
  ROUTER --> RETRY --> GEN --> DEB
  LGBM --> QPRED --> MET

  DEB -->|SUPPORTED| API
  DEB -->|else| REF["Refuse — do not guess"]
  REF --> API
  MET --> API
  API --> UI

  style IN fill:#020617,stroke:#22d3ee,color:#e2e8f0
  style PREP fill:#042f2e,stroke:#2dd4bf,color:#e2e8f0
  style STORE fill:#1e1b4b,stroke:#a78bfa,color:#e2e8f0
  style THINK fill:#0f172a,stroke:#38bdf8,color:#e2e8f0
  style CHECK fill:#3f1d2e,stroke:#f472b6,color:#e2e8f0
  style SERVE fill:#052e16,stroke:#4ade80,color:#e2e8f0
```

```text
DocuVerify path     docs → chunks → BM25+dense → agent → DeBERTa → FastAPI → TypeScript
Forecasting path    series → causal features → LightGBM quantiles → metrics → FastAPI → TypeScript
Shared rule         if the check fails, the UI shows the failure
```

---

<div align="center">

## stack I live in

<img src="https://skillicons.dev/icons?i=python,typescript,pytorch,react,fastapi,docker,aws,azure,linux,git,github,vscode" alt="stack"/>

</div>

<br/>

**languages** — Python · TypeScript · Java · SQL  
**ai / ml** — RAG · FastAPI · REST APIs · NLP · feature engineering · evaluation  
**libs** — PyTorch · Hugging Face · LightGBM · Scikit-learn · NumPy · Pandas  
**ship** — Git · Linux · Docker · AWS · Azure

---

<div align="center">

## contribution snake

the grid, eaten in order

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/devcodes007/devcodes007/output/github-contribution-grid-snake-dark.svg" />
  <img alt="github contribution snake" src="https://raw.githubusercontent.com/devcodes007/devcodes007/output/github-snake-green.svg" />
</picture>

</div>

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=devcodes007&show_icons=true&theme=radical&hide_border=true&bg_color=020617&title_color=22d3ee&icon_color=22d3ee&text_color=e2e8f0" height="165" alt="stats"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=devcodes007&theme=radical&hide_border=true&background=020617&ring=22d3ee&fire=22d3ee&currStreakLabel=22d3ee" height="165" alt="streak"/>

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:22d3ee,50:0e7490,100:020617&height=140&section=footer&text=retrieve%20%C2%B7%20verify%20%C2%B7%20ship&fontSize=22&fontColor=F8FAFC&animation=twinkling" width="100%" alt="footer"/>
</div>
