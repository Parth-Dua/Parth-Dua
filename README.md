<h1 align="center">Parth Dua</h1>

<p align="center">
  <b>I build AI agents and ML systems that have to be right, not just plausible.</b><br>
  MS CS @ UCLA &nbsp;·&nbsp; BS CS (Honors) @ UMD, 3.97 GPA &nbsp;·&nbsp; ML research on NASA GPM satellite data &nbsp;·&nbsp; computational biology preprint co-author
</p>

<p align="center">
  <a href="https://linkedin.com/in/parth-dua">LinkedIn</a> &nbsp;·&nbsp;
  <a href="https://devpost.com/parthdua2005">Devpost</a> &nbsp;·&nbsp;
  <a href="mailto:parth.dua.tech@gmail.com">parth.dua.tech@gmail.com</a>
</p>

<p align="center">
  <a href="#featured-builds">Featured builds</a> &nbsp;|&nbsp;
  <a href="#more-builds">More builds</a> &nbsp;|&nbsp;
  <a href="#research-and-experience">Research and experience</a> &nbsp;|&nbsp;
  <a href="#stack">Stack</a>
</p>

---

**What I work on**

- **Agents with guardrails:** the LLM interprets, deterministic code owns money, time, and permissions, and humans approve what matters.
- **Retrieval you can trust:** hybrid search, reranking, and reliability layers, evaluated on 500K-document benchmarks.
- **ML on messy real-world signals:** satellite radar, UWB + LiDAR SLAM, and 120K-tree phylogenetic simulations.

## Featured builds

### 1. [Breakwater](https://github.com/Parth-Dua/breakwater-submission) &nbsp;·&nbsp; Cal Hacks 13.0

**A self-improving demurrage desk that reconciles vessel telemetry with enterprise accounting.**

When a ship overstays its port contract, money is owed in two directions. Breakwater checks the delay against vessel telemetry and the contract PDFs, calculates both claims, routes decisions to the right person, and posts balanced journals. Human corrections become approved, scoped procedures instead of silent behavior changes.

- Deterministic time and money engines (integer minutes and cents), verbatim-quote checks on every extracted fact, role-gated approvals, SHA-256 audit chain
- Learning loop compares the agent's trace with what humans actually did, then backtests each proposed procedure on historical voyages before it can run

`Next.js` `TypeScript` `Convex` `Claude` `LangChain` `MapLibre`

[Devpost](https://devpost.com/software/breakwater-46yk7q) &nbsp;·&nbsp; [Demo video](https://youtu.be/MlzrFt0Pl9k) &nbsp;·&nbsp; [Code](https://github.com/Parth-Dua/breakwater-submission)

### 2. [Parley](https://github.com/Parth-Dua/freight-recovery-exchange) &nbsp;·&nbsp; LA Hacks AI Hackathon 2026

**An autonomous freight market where AI agents negotiate privately and coordinate recovery when shipping is disrupted.**

- Shippers book entirely inside ASI:One: a private buyer agent negotiates with five independent carrier uAgents in parallel without revealing its budget, then pays through the Fetch Agent Payment Protocol and Stripe
- When a carrier withdraws a sailing, every stranded booking is renegotiated at once and cleared jointly by a five-stage lexicographic OR-Tools objective, benchmarked against first-come-first-served
- Slot-level locking in TimescaleDB means parallel agents can never oversell; every step is recorded and replayable in Mission Control

`Python` `Fetch.ai uAgents` `ASI:One` `OR-Tools` `TimescaleDB` `React`

[Devpost](https://devpost.com/software/project-ert3qi512sok) &nbsp;·&nbsp; [Code](https://github.com/Parth-Dua/freight-recovery-exchange)

### 3. [AnchorVision](https://github.com/Loldude0/AnchorVision) &nbsp;·&nbsp; UMD x Ironsite Startup Shell Hackathon

**UWB-anchored LiDAR SLAM that turns construction walkthroughs into one searchable 4D site map.**

- Aligns separate worker walkthroughs in a shared site frame without GPS or overlapping paths by solving the transform over sparse UWB ranges
- Ray-casts YOLO detections into the point cloud so every object carries a 3D location and a timestamp
- Answers questions like *"what changed in this hallway between 8 and 10 AM?"* with a vision language model grounded in a retrieval index

`Python` `RGB-D SLAM` `UWB` `YOLO` `VLM`

[Devpost](https://devpost.com/software/anchorvision) &nbsp;·&nbsp; [Code](https://github.com/Loldude0/AnchorVision)

### 4. [TemporalGuard](https://github.com/Parth-Dua/TemporalGuard)

**A pre-generation reliability layer that teaches cheap RAG when to answer, abstain, or flag a conflict.**

- Indexed EnterpriseRAG-Bench (512K documents) on Modal GPUs; hybrid dense + BM25 search with cross-encoder reranking lifted recall from **50% to 88%**
- Gates every response as `ANSWER` / `NOT_FOUND` / `ABSTAIN` / `CONFLICT`, cutting unsupported answers from **25% to 17.5%** and improving conflict detection **60%**
- Caching deterministic LLM calls by input hash cut repeat evaluation cost **97%**

`Python` `FAISS` `sentence-transformers` `Modal` `LangChain`

[Code](https://github.com/Parth-Dua/TemporalGuard)

## More builds

| Project | What it does | Built at |
|---|---|---|
| [RAID](https://github.com/Parth-Dua/RAID) | Real-time multiplayer incident-response simulator. Each engineer sees different logs and metrics, and an AI game master nudges the team without solving it. | Personal project |
| [TriageNav](https://github.com/Parth-Dua/RiageNav) | Voice or text symptom triage with Claude that ranks nearby care on a live crowding and distance map. | Anthropic x Maryland · [Devpost](https://devpost.com/software/triagenav) |
| [PlatePal](https://github.com/tranade/plate-pal) | Campus marketplace for sharing surplus groceries. 🏆 **Environmental Track** and 🏆 **Best Domain Name**. | Hoya Hacks 2024 · [Devpost](https://devpost.com/software/platepal-ek60rc) |
| [CrowdCure](https://github.com/virsgandhi20/HopHacks24-Parth-Vir) | Estimates hospital crowding from WiFi signals to route patients to shorter waits. | HopHacks 2024 · [Devpost](https://devpost.com/software/crowdcure) |

## Research and experience

- **ML Research Intern, Cooperative Institute for Satellite Earth System Studies:** low-cost ResNet alternative to radar retrievals for NASA GPM, 3x faster GPU pipelines over multi-TB HDF5, and a two-stage classifier-regressor that fixed model collapse on a 96/4 class imbalance
- **Undergraduate Researcher, Molloy Lab (UMD):** built the first end-to-end empirical evaluation of ASTRAL-Pro tagging, covering 120K gene trees across 60 SLURM experiments. [Preprint](https://doi.org/10.64898/2026.01.20.700722), with posters at WABI and SURC
- **Team Lead, Engineering Digital Services (UMD):** led 8 engineers on Pinpoint, the management system for 50+ makerspaces, and automated 40% of low-risk approvals with CODEOWNERS and GitHub Actions
- **Software Intern, Tech Mahindra:** eliminated $25K+ a month in idle cloud spend with an automated AWS-Nuke pipeline and migrated 4 enterprise apps to AWS using Jenkins and Terraform

## Stack

**Languages:** Python · TypeScript · Java · C · Rust · SQL<br>
**AI / ML:** PyTorch · LangChain · OpenAI Agents SDK · Claude API · FAISS · scikit-learn<br>
**Web / Infra:** React · Next.js · Flask · Django · Docker · AWS · Terraform · Modal · Convex
