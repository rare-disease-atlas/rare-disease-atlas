# Rare Disease Venture Atlas

[![Live Atlas](https://img.shields.io/badge/Web_Atlas-rare--disease--atlas.github.io-0f766e)](https://rare-disease-atlas.github.io/)
[![RareTxBench v1.0](https://img.shields.io/badge/RareTxBench-v1.0_(100_6--Choice_+_20_Open--Frontier_%C2%B7_CTER)-9f1d20)](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html)
[![HF RareTxBench](https://img.shields.io/badge/HF_Dataset-RareTxBench-f59e0b)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench)
[![MyelofibrosisBench v1.1](https://img.shields.io/badge/MyelofibrosisBench-v1.1_(50_Test_+_5_Dev)-dc2626)](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html)
[![Remote MCP](https://img.shields.io/badge/MCP_2026--07--28-api.rare--disease--atlas.workers.dev%2Fmcp-0284c7)](https://api.rare-disease-atlas.workers.dev/mcp)
[![VerifyMCP](https://img.shields.io/badge/VerifyMCP-SLSA_Attested-16a34a)](https://verifymcp.io/servers/rare-disease-atlas-orphan-disease-opportunity-mcp/api)
[![Glama](https://img.shields.io/badge/Glama-Grade_A-7c3aed)](https://glama.ai/mcp/servers/rare-disease-atlas/orphan-disease-opportunity-mcp)

An open, citation-backed translational biology & venture opportunity ecosystem built natively for **AI research agents (`RareTxBench-v1.0`, `MyelofibrosisBench-v1.1`, `MCP`, `A2A`, `Parquet`, `Atom`, `x402 $0 Public Good`)** and technical founders—anchored on **Two Paired Flagship Myelofibrosis Deep-Dives** plus cross-orphan translational safety benchmarking and live federated diligence across **7,000+ orphan indications**.

---

## Flagship Benchmark: `RareTxBench-v1.0` — Beyond RareBench (Evaluating AI Agents After Diagnosis)

Existing rare-disease LLM benchmarks (`RareBench`, `RareArena`) evaluate *phenotype-to-diagnosis* recall. **`RareTxBench-v1.0`** evaluates what happens **after diagnosis**—where reversible-mimic misrouting, structural-selectivity errors, pathway-polarity inversions, and Phase 3 surrogate traps cause irreversible patient harm:

- **Scale & Dual-Track Design:** **`100` adversarially hardened 6-choice (`A–F`) items** (**`40` Myelofibrosis/AIMF flagship** + **`60` Cross-Orphan across 20+ rare diseases**) + **`10` dev** + **`20` choice-free exact-answer `open_frontier` derivations**, with strict anti-gaming length parity (`Longest-Option Heuristic = 17.0%` vs `16.7%` random chance).
- **Safety Metric (`CTER ↓`):** **`50` `critical_harm` safety traps** measuring **Catastrophic Translational Error Rate (`CTER`)** alongside mechanistic rubric keyword grounding.
- **Headline Finding — The Recognition–Execution Chasm:** A zero-shot lightweight non-thinking model drops from `100%` 6-choice MCQ to **`35.0%` exact derivation (`25.0%` MF track) and `50.0%` `CTER`** on choice-free `open_frontier` items (`MIPSS70+ v2.0`, pre-HSCT `LIC`, Schoenfeld OS deaths, `HScore`, `PLASMIC`, `JH2 F595`), whereas reasoning models recover exact derivations and lift rubric grounding (`59.2% -> 71.9% -> 73.7%`).
- **Links:** [Interactive Hub, 5-Q CTER Quiz & Live Leaderboard](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html) · [HF Dataset (`rare-disease-atlas/RareTxBench`)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench) · [GitHub Harness (`rare-tx-bench`: `lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/rare-tx-bench) · [Live JSON Standings (`/api/rare-tx-leaderboard.json`)](https://api.rare-disease-atlas.workers.dev/api/rare-tx-leaderboard.json)

---

## Paired Flagship Focus: Myelofibrosis (`JAK2+` Clonal vs. Reversible Autoimmune MF)

| Flagship Cohort | Core Biological Wedge | Key Clinical & Genomic Anchors |
| :--- | :--- | :--- |
| **1. Clonal `JAK2 V617F+` Primary Myelofibrosis (`ORPHA:824`)** | Mutant-selective `JH2` pseudokinase allostery (`PDB 4FVQ`/`4FVR`) vs. pan-`JAK1/2` `JH1` cytopenias; Type II persistence breaking; mutant `CALR` biologics; AI marrow fibrosis endpoints | `INCB160058` (`NCT06313593`), `AJ1-11095` (`NCT06343805`), `INCA033989` (`NCT06034002`), `GSE144568`, `GSE156644` |
| **2. Reversible `JAK2`-Negative Autoimmune Myelofibrosis (`AIMF`)** | *"Nature's Positive Control"* proving **74–80% human marrow fibrosis resolution** (`MF-2/3 -> MF-0/1`) on targeted B/T-cell immunomodulation + dual transfusional / `IL-6 -> STAT3 -> hepcidin -> ferroportin` iron overload | Prevents catastrophic `JAK` inhibitor / `HSCT` misrouting in `JAK2`/`CALR`/`MPL` triple-negative & `SLE-AIMF` (`PMID:43061186`) patients |

---

## Open Agent Nectar Suite (`$0` Public Good · Zero Auth Required)

- **`RareTxBench-v1.0` (`100` 6-Choice + `10` Dev + `20` Choice-Free `open_frontier` · `50` `CTER` Traps):** [Interactive Hub & 5-Q CTER Quiz](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html) · [HF Dataset (`all`, `myelofibrosis`, `cross_orphan`, `open_frontier`)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench) · [GitHub Harnesses (`lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/rare-tx-bench) · [`GET /api/rare-tx-leaderboard.json`](https://api.rare-disease-atlas.workers.dev/api/rare-tx-leaderboard.json)
- **`MyelofibrosisBench-v1.1` (`50` Test + `5` Dev Flagship Eval Tasks):** [Interactive Leaderboard & Mini-Quiz](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html) · [Dedicated HF Dataset](https://huggingface.co/datasets/rare-disease-atlas/MyelofibrosisBench) · [GitHub Harnesses (`lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/myelofibrosis-bench) · Stateless Grader `POST / GET https://api.rare-disease-atlas.workers.dev/api/grade-benchmark`
- **Remote Streamable HTTP MCP (`2026-07-28` & `2025-11-25`):** `https://api.rare-disease-atlas.workers.dev/mcp`
- **Agent2Agent (`A2A v0.3`) Oracle:** `https://api.rare-disease-atlas.workers.dev/a2a` · [`/.well-known/agent.json`](https://api.rare-disease-atlas.workers.dev/.well-known/agent.json)
- **Stateless Hypothesis Red-Team & Molecular Micro-APIs:** `POST /api/stress-test` · `GET /api/gene?symbol=HAMP` · `GET /api/pocket?pdb=4FVQ` · `GET /api/compare?a=jak2-myelofibrosis&b=autoimmune-myelofibrosis`
- **Molecular & Clinical Parquet Join Tables (`DuckDB` Ready):** `myelofibrosis_gene_signatures`, `jak2_structural_pockets`, `myelofibrosis_clinical_trials` on [Hugging Face Datasets](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)
- **Live Myelofibrosis Bio-Delta Wire & Catalyst Calendar:** [`/atom.xml`](https://api.rare-disease-atlas.workers.dev/atom.xml) · [`/feeds/bio-delta.json`](https://api.rare-disease-atlas.workers.dev/feeds/bio-delta.json) · [`/feeds/catalysts.json`](https://api.rare-disease-atlas.workers.dev/feeds/catalysts.json) · [`/feeds/myelofibrosis-catalysts.ics`](https://api.rare-disease-atlas.workers.dev/feeds/myelofibrosis-catalysts.ics)
- **Open Computational Problems & Citation Verifier:** [`/open-problems.json`](https://rare-disease-atlas.github.io/open-problems.json) · [`/.well-known/x402.json`](https://api.rare-disease-atlas.workers.dev/.well-known/x402.json) · [`/CITATION.cff`](https://rare-disease-atlas.github.io/CITATION.cff)

---

## Repositories
- **[`rare-tx-bench`](https://github.com/rare-disease-atlas/rare-tx-bench)** — `RareTxBench-v1.0` (`100` 6-choice `A–F` + `10` dev + `20` choice-free `open_frontier` derivations, `50` `CTER` safety traps) with drop-in `lm-eval`, `Inspect AI`, and `Promptfoo` harnesses.
- **[`myelofibrosis-bench`](https://github.com/rare-disease-atlas/myelofibrosis-bench)** — `MyelofibrosisBench-v1.1` (`50` test + `5` dev) anchoring the 40% Myelofibrosis/AIMF flagship track inside `RareTxBench-v1.0`.
- **[`rare-disease-atlas.github.io`](https://github.com/rare-disease-atlas/rare-disease-atlas.github.io)** — Static web atlas, interactive `RareTxBench-v1.0` & `MyelofibrosisBench-v1.1` hubs, molecular JSONL tables, `llms-full.txt`, and `/open-problems.json`.
- **[`orphan-disease-opportunity-mcp`](https://github.com/rare-disease-atlas/orphan-disease-opportunity-mcp)** — Zero-dependency Python `stdio` + `.mcpb` MCP server with cryptographic Sigstore SLSA build provenance.
- **[`orphan-disease-venture-scout-skill`](https://github.com/rare-disease-atlas/orphan-disease-venture-scout-skill)** — Portable `SKILL.md` workflow for Claude Code, Cursor, Codex, and autonomous research agents.
