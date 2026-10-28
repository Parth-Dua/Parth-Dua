<h1 align="center">Parth Dua</h1>

<p align="center">MS CS @ UCLA &nbsp;·&nbsp; 3.97 GPA @ UMD</p>

<p align="center"><samp>
  <a href="https://www.overleaf.com/project/6a8343a0de4ed3740ebd2c47/share#ab26f9b1148f83dcc336ca94c4349cb32cd7e961bf9069e6">resume</a> &nbsp;·&nbsp;
  <a href="https://linkedin.com/in/parth-dua">linkedin</a> &nbsp;·&nbsp;
  parth.dua.tech@gmail.com
</samp></p>

---

I like taking what I know into new domains, from shipping and finance to construction and healthcare, and building things that make a real difference for the people who use them.

## Featured builds

### 1. [Breakwater](https://github.com/Parth-Dua/breakwater-submission) &nbsp;·&nbsp; Cal Hacks 13.0

**A self-improving demurrage desk that reconciles vessel telemetry with enterprise accounting.**

- Checks port delays against vessel telemetry and contract PDFs, calculates the claims owed in both directions, routes decisions to the right person, and posts balanced journals
- Deterministic time and money engines, verbatim-quote checks on every extracted fact, role-gated approvals, and a SHA-256 audit chain
- Learns from human corrections by comparing its trace with what people actually did, then backtests each new procedure on past voyages before it can run

`Next.js` `TypeScript` `Convex` `Claude` `LangChain` `MapLibre`

### 2. [Parley](https://github.com/Parth-Dua/freight-recovery-exchange) &nbsp;·&nbsp; LA Hacks AI Hackathon 2026

**An autonomous freight market where AI agents negotiate privately and coordinate recovery when shipping is disrupted.**

- Shippers book entirely inside ASI:One: a private buyer agent negotiates with five carrier agents in parallel without revealing its budget, then pays through the Fetch Agent Payment Protocol and Stripe
- When a sailing is withdrawn, every stranded booking is renegotiated at once and cleared jointly by a five-stage OR-Tools objective, benchmarked against first-come-first-served
- Slot-level locking in TimescaleDB means parallel agents can never oversell; every step is replayable in Mission Control

`Python` `Fetch.ai uAgents` `ASI:One` `OR-Tools` `TimescaleDB` `React`

### 3. [TemporalGuard](https://github.com/Parth-Dua/TemporalGuard)

**An eval-driven RAG project: five iterations teaching a cheap pipeline when to answer, abstain, or flag a conflict.**

- Ran every version on EnterpriseRAG-Bench (512K documents), changing one thing at a time and tracing each failure to retrieval, chunking, or the decision step
- Hybrid BM25 + dense retrieval and structure-aware chunking lifted recall@5 from **50% to 88%**
- A pre-generation conflict layer raised safe-decision accuracy from **41% to 77%** and conflict detection from **0% to 60%**, while cutting unsupported answers from 25% to 17.5%

`Python` `FAISS` `BM25` `bge-small` `Modal` `DeepSeek`

### 4. [AnchorVision](https://github.com/Loldude0/AnchorVision) &nbsp;·&nbsp; UMD x Ironsite Startup Shell Hackathon

**UWB-anchored LiDAR SLAM that turns construction walkthroughs into one searchable 4D site map.**

- Aligns separate worker walkthroughs in a shared site frame without GPS or overlapping paths by solving the transform over sparse UWB ranges
- Ray-casts YOLO detections into the point cloud so every object carries a 3D location and a timestamp
- Answers questions like *"what changed in this hallway between 8 and 10 AM?"* with a vision language model grounded in a retrieval index

`Python` `RGB-D SLAM` `UWB` `YOLO` `VLM`

## More builds

| Project | What it does | Event |
|---|---|---|
| [TriageNav](https://github.com/Parth-Dua/RiageNav) | Voice or text symptom triage with Claude that ranks nearby care on a live crowding and distance map | Anthropic x Maryland Hackathon |
| [PlatePal](https://github.com/tranade/plate-pal) | Campus marketplace for sharing surplus groceries. 🏆 Environmental Track, 🏆 Best Domain Name | Hoya Hacks 2024 |
| [CrowdCure](https://github.com/virsgandhi20/HopHacks24-Parth-Vir) | Estimates hospital crowding from WiFi signals to route patients to shorter waits | HopHacks 2024 |

## Stack

<table>
  <tr><td><b>Languages</b></td><td>Python, TypeScript, JavaScript, Java, C, Rust, SQL</td></tr>
  <tr><td><b>ML</b></td><td>PyTorch, scikit-learn, FAISS, YOLO, OR-Tools</td></tr>
  <tr><td><b>LLMs & agents</b></td><td>Claude API, OpenAI Agents SDK, LangChain, LangGraph, Fetch.ai uAgents</td></tr>
  <tr><td><b>Web</b></td><td>React, Next.js, Node.js, Flask, Django, Tailwind</td></tr>
  <tr><td><b>Data & infra</b></td><td>PostgreSQL / TimescaleDB, Convex, Docker, AWS, Terraform, Modal, GitHub Actions</td></tr>
</table>
