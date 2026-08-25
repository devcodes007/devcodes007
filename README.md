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

I do not collect tutorials. I pick a failure I can measure, then force it through every layer of the stack until a UI can show the miss.

```mermaid
flowchart TB
  subgraph L0["L0 · FAILURE SURFACE — what I hunt"]
    F1["unsupported RAG claim"]
    F2["leaky time-series feature"]
    F3["Gujarat regime shift"]
    F4["P10/P50/P90 crossing"]
  end

  subgraph L1["L1 · PROBLEM FRAME — write the contract"]
    P1["question type<br/>lookup / compare / multi-hop"]
    P2["prediction type<br/>quantile, not a point"]
    P3["forbidden cheats<br/>no future lags · no test shopping"]
    P4["success = a metric that can fail"]
  end

  subgraph L2["L2 · DATA PLANE"]
    D1["PDFs / markdown<br/>document_id forever"]
    D2["daily demand · weather · holiday<br/>10k+ state-grouped rows"]
    D3["chronological cuts<br/>train / val / test"]
    D4["document-level splits<br/>never split the same doc"]
  end

  subgraph L3["L3 · REPRESENTATION"]
    R1["structure-aware chunks<br/>heading path + metadata"]
    R2["causal lags + rolling<br/>shift 1 by state"]
    R3["EWMA residual<br/>alpha chosen on val only"]
    R4["schemas<br/>question · evidence · forecast"]
  end

  subgraph L4["L4 · INDEX + MODEL"]
    I1["BM25<br/>identifier tokenizer"]
    I2["dense embed<br/>Chroma / MiniLM"]
    I3["hybrid score<br/>minmax then mix"]
    I4["LightGBM<br/>P10 · P50 · P90"]
  end

  subgraph L5["L5 · CONTROL PLANE — agents and selection"]
    C1["query router"]
    C2["evidence evaluator"]
    C3["reformulate + retry ≤ 3"]
    C4["alpha sweep 0 / 0.25 / 0.5 / 0.75 / 1"]
    C5["pick on validation only"]
  end

  subgraph L6["L6 · GENERATION / INFERENCE"]
    G1["evidence-only prompt<br/>citations required"]
    G2["one-step quantile infer<br/>same features as train"]
    G3["SSE agent trace<br/>classification → retrieve → verify"]
  end

  subgraph L7["L7 · SECOND OPINION — do not trust the first model"]
    V1["DeBERTa-v3-small<br/>SUPPORTED / CONTRADICTED / UNSUPPORTED"]
    V2["pinball + coverage"]
    V3["crossing rate ~12%"]
    V4["shift: train ~310 vs val ~373"]
    V5["refuse if unsupported"]
  end

  subgraph L8["L8 · PLATFORM"]
    A1["FastAPI REST"]
    A2["Pydantic contracts"]
    A3["ingest / query / predict / metrics"]
    A4["errors over invented history"]
  end

  subgraph L9["L9 · EXPERIENCE"]
    U1["TypeScript client"]
    U2["live answer + citations"]
    U3["groundedness chip"]
    U4["P10-P90 band + shift panel"]
  end

  subgraph L10["L10 · FEEDBACK — the loop closes"]
    X1["what the UI made obvious"]
    X2["new failure becomes L0"]
  end

  F1 --> P1
  F2 --> P3
  F3 --> P2
  F4 --> P4

  P1 --> D1
  P2 --> D2
  P3 --> D3
  P4 --> D4

  D1 --> R1
  D2 --> R2
  D3 --> R3
  D4 --> R4

  R1 --> I1
  R1 --> I2
  I1 --> I3
  I2 --> I3
  R2 --> I4
  R3 --> I4
  R4 --> A2

  I3 --> C1
  C1 --> C2 --> C3
  I4 --> C4 --> C5

  C3 --> G1
  C5 --> G2
  G1 --> G3

  G1 --> V1
  G2 --> V2
  V2 --> V3
  V2 --> V4
  V1 --> V5

  V5 --> A1
  V3 --> A3
  V4 --> A3
  A2 --> A1
  A1 --> A3
  A3 --> A4

  A1 --> U1
  G3 --> U2
  V1 --> U3
  V3 --> U4
  U1 --> U2
  U1 --> U3
  U1 --> U4

  U2 --> X1
  U3 --> X1
  U4 --> X1
  X1 --> X2
  X2 --> F1
  X2 --> F2
  X2 --> F3
  X2 --> F4

  style L0 fill:#1a0b10,stroke:#fb7185,color:#e2e8f0
  style L1 fill:#0b1220,stroke:#22d3ee,color:#e2e8f0
  style L2 fill:#052e2b,stroke:#2dd4bf,color:#e2e8f0
  style L3 fill:#1e1b4b,stroke:#a78bfa,color:#e2e8f0
  style L4 fill:#0f172a,stroke:#38bdf8,color:#e2e8f0
  style L5 fill:#172554,stroke:#60a5fa,color:#e2e8f0
  style L6 fill:#3b0764,stroke:#e879f9,color:#e2e8f0
  style L7 fill:#4a1c2a,stroke:#f472b6,color:#e2e8f0
  style L8 fill:#052e16,stroke:#4ade80,color:#e2e8f0
  style L9 fill:#083344,stroke:#67e8f9,color:#e2e8f0
  style L10 fill:#020617,stroke:#fbbf24,color:#e2e8f0
```

Eleven layers. Same loop as before — just the real machine behind it.

| layer | job |
| :--- | :--- |
| **L0 failure** | Name the miss: hallucination, leak, shift, crossing. |
| **L1 contract** | Question type, quantile type, cheats that are illegal. |
| **L2 data** | Document IDs and chronological cuts stay glued to every row. |
| **L3 representation** | Chunks + causal features + schemas. |
| **L4 index / model** | BM25 + dense hybrid, or LightGBM P10/P50/P90. |
| **L5 control** | Router, evidence retries, validation-only selection. |
| **L6 inference** | Evidence-only generation or one-step quantiles + SSE. |
| **L7 second opinion** | DeBERTa or pinball/coverage/crossing — then refuse. |
| **L8 platform** | FastAPI, Pydantic, real error paths. |
| **L9 UI** | TypeScript shows refuse / band / shift. |
| **L10 feedback** | Whatever the UI made obvious becomes the next L0. |

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
