# Rare Disease Venture Atlas

[![Live Atlas](https://img.shields.io/badge/Web_Atlas-rare--disease--atlas.github.io-0f766e)](https://rare-disease-atlas.github.io/)
[![MyelofibrosisBench v1.1](https://img.shields.io/badge/MyelofibrosisBench-v1.1_(50_Test_+_5_Dev)-dc2626)](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html)
[![HF Benchmark](https://img.shields.io/badge/HF_Dataset-MyelofibrosisBench-f59e0b)](https://huggingface.co/datasets/rare-disease-atlas/MyelofibrosisBench)
[![Remote MCP](https://img.shields.io/badge/MCP_2026--07--28-api.rare--disease--atlas.workers.dev%2Fmcp-0284c7)](https://api.rare-disease-atlas.workers.dev/mcp)
[![VerifyMCP](https://img.shields.io/badge/VerifyMCP-SLSA_Attested-16a34a)](https://verifymcp.io/servers/rare-disease-atlas-orphan-disease-opportunity-mcp/api)
[![Glama](https://img.shields.io/badge/Glama-Grade_A-7c3aed)](https://glama.ai/mcp/servers/rare-disease-atlas/orphan-disease-opportunity-mcp)

An open, citation-backed translational biology & venture opportunity ecosystem built natively for **AI research agents (`MCP`, `A2A`, `MyelofibrosisBench-v1.1`, `Parquet`, `Atom`, `x402 $0 Public Good`)** and technical founders—anchored on **Two Paired Flagship Myelofibrosis Deep-Dives** plus live federated diligence across **7,000+ orphan indications**.

---

## Paired Flagship Focus: Myelofibrosis (`JAK2+` Clonal vs. Reversible Autoimmune MF)

| Flagship Cohort | Core Biological Wedge | Key Clinical & Genomic Anchors |
| :--- | :--- | :--- |
| **1. Clonal `JAK2 V617F+` Primary Myelofibrosis (`ORPHA:824`)** | Mutant-selective `JH2` pseudokinase allostery (`PDB 4FVQ`/`4FVR`) vs. pan-`JAK1/2` `JH1` cytopenias; Type II persistence breaking; mutant `CALR` biologics; AI marrow fibrosis endpoints | `INCB160058` (`NCT06313593`), `AJ1-11095` (`NCT06343805`), `INCA033989` (`NCT06034002`), `GSE144568`, `GSE156644` |
| **2. Reversible `JAK2`-Negative Autoimmune Myelofibrosis (`AIMF`)** | *"Nature's Positive Control"* proving **74–80% human marrow fibrosis resolution** (`MF-2/3 -> MF-0/1`) on targeted B/T-cell immunomodulation + dual transfusional / `IL-6 -> STAT3 -> hepcidin -> ferroportin` iron overload | Prevents catastrophic `JAK` inhibitor / `HSCT` misrouting in `JAK2`/`CALR`/`MPL` triple-negative & `SLE-AIMF` (`PMID:43061186`) patients |

---

## Open Agent Nectar Suite (`$0` Public Good · Zero Auth Required)

- **`MyelofibrosisBench-v1.1` (`50` Test + `5` Dev Ground-Truth Eval Tasks):** [Interactive Leaderboard & Mini-Quiz](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html) · [Dedicated HF Dataset](https://huggingface.co/datasets/rare-disease-atlas/MyelofibrosisBench) · [GitHub Harnesses (`lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/myelofibrosis-bench) · Stateless Grader `POST / GET https://api.rare-disease-atlas.workers.dev/api/grade-benchmark`
- **Remote Streamable HTTP MCP (`2026-07-28` & `2025-11-25`):** `https://api.rare-disease-atlas.workers.dev/mcp`
- **Agent2Agent (`A2A v0.3`) Oracle:** `https://api.rare-disease-atlas.workers.dev/a2a` · [`/.well-known/agent.json`](https://api.rare-disease-atlas.workers.dev/.well-known/agent.json)
- **Stateless Hypothesis Red-Team & Molecular Micro-APIs:** `POST /api/stress-test` · `GET /api/gene?symbol=HAMP` · `GET /api/pocket?pdb=4FVQ` · `GET /api/compare?a=jak2-myelofibrosis&b=autoimmune-myelofibrosis`
- **Molecular & Clinical Parquet Join Tables (`DuckDB` Ready):** `myelofibrosis_gene_signatures`, `jak2_structural_pockets`, `myelofibrosis_clinical_trials` on [Hugging Face Datasets](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)
- **Live Myelofibrosis Bio-Delta Wire & Catalyst Calendar:** [`/atom.xml`](https://api.rare-disease-atlas.workers.dev/atom.xml) · [`/feeds/bio-delta.json`](https://api.rare-disease-atlas.workers.dev/feeds/bio-delta.json) · [`/feeds/catalysts.json`](https://api.rare-disease-atlas.workers.dev/feeds/catalysts.json) · [`/feeds/myelofibrosis-catalysts.ics`](https://api.rare-disease-atlas.workers.dev/feeds/myelofibrosis-catalysts.ics)
- **Open Computational Problems & Citation Verifier:** [`/open-problems.json`](https://rare-disease-atlas.github.io/open-problems.json) · [`/.well-known/x402.json`](https://api.rare-disease-atlas.workers.dev/.well-known/x402.json) · [`/CITATION.cff`](https://rare-disease-atlas.github.io/CITATION.cff)

---

## Repositories
- **[`myelofibrosis-bench`](https://github.com/rare-disease-atlas/myelofibrosis-bench)** — `MyelofibrosisBench-v1.1` (`50` test + `5` dev) with drop-in harnesses for EleutherAI `lm-evaluation-harness`, UK AISI `Inspect AI`, and `Promptfoo`.
- **[`rare-disease-atlas.github.io`](https://github.com/rare-disease-atlas/rare-disease-atlas.github.io)** — Static web atlas, interactive `MyelofibrosisBench-v1.1` leaderboard & mini-quiz, molecular JSONL tables, `llms-full.txt`, and `/open-problems.json`.
- **[`orphan-disease-opportunity-mcp`](https://github.com/rare-disease-atlas/orphan-disease-opportunity-mcp)** — Zero-dependency Python `stdio` + `.mcpb` MCP server with cryptographic Sigstore SLSA build provenance.
- **[`orphan-disease-venture-scout-skill`](https://github.com/rare-disease-atlas/orphan-disease-venture-scout-skill)** — Portable `SKILL.md` workflow for Claude Code, Cursor, Codex, and autonomous research agents.
