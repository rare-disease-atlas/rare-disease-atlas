# Rare Disease Venture Atlas

[![Live Atlas](https://img.shields.io/badge/Web_Atlas-rare--disease--atlas.github.io-0f766e)](https://rare-disease-atlas.github.io/)
[![Remote MCP](https://img.shields.io/badge/MCP_2026--07--28-api.rare--disease--atlas.workers.dev%2Fmcp-0284c7)](https://api.rare-disease-atlas.workers.dev/mcp)
[![VerifyMCP](https://img.shields.io/badge/VerifyMCP-SLSA_Attested-16a34a)](https://verifymcp.io/servers/rare-disease-atlas-orphan-disease-opportunity-mcp/api)
[![Glama](https://img.shields.io/badge/Glama-Grade_A-7c3aed)](https://glama.ai/mcp/servers/rare-disease-atlas/orphan-disease-opportunity-mcp)
[![HF Dataset](https://img.shields.io/badge/Hugging_Face-10_Parquet_Configs_%26_MyelofibrosisBench-f59e0b)](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)

An open, citation-backed translational biology & venture opportunity ecosystem built natively for **AI research agents (`MCP`, `A2A`, `MyelofibrosisBench-v1`, `Parquet`, `Atom`, `x402 $0 Public Good`)** and technical founders—anchored on **Two Paired Flagship Myelofibrosis Deep-Dives** plus live federated diligence across **7,000+ orphan indications**.

---

## Paired Flagship Focus: Myelofibrosis (`JAK2+` Clonal vs. Reversible Autoimmune MF)

| Flagship Cohort | Core Biological Wedge | Key Clinical & Genomic Anchors |
| :--- | :--- | :--- |
| **1. Clonal `JAK2 V617F+` Primary Myelofibrosis (`ORPHA:824`)** | Mutant-selective `JH2` pseudokinase allostery (`PDB 4FVQ`/`4FVR`) vs. pan-`JAK1/2` `JH1` cytopenias; Type II persistence breaking; mutant `CALR` biologics; AI marrow fibrosis endpoints | `INCB160058` (`NCT06313593`), `AJ1-11095` (`NCT06343805`), `INCA033989` (`NCT06034002`), `GSE144568`, `GSE156644` |
| **2. Reversible `JAK2`-Negative Autoimmune Myelofibrosis (`AIMF`)** | *"Nature's Positive Control"* proving **74–80% human marrow fibrosis resolution** (`MF-2/3 -> MF-0/1`) on targeted B/T-cell immunomodulation + dual transfusional / `IL-6 -> STAT3 -> hepcidin -> ferroportin` iron overload | Prevents catastrophic `JAK` inhibitor / `HSCT` misrouting in `JAK2`/`CALR`/`MPL` triple-negative patients |

---

## Open Agent Nectar Suite (`$0` Public Good · Zero Auth Required)

- **Remote Streamable HTTP MCP (`2026-07-28` & `2025-11-25`):** `https://api.rare-disease-atlas.workers.dev/mcp`
- **Agent2Agent (`A2A v0.3`) Oracle:** `https://api.rare-disease-atlas.workers.dev/a2a` · [`/.well-known/agent.json`](https://api.rare-disease-atlas.workers.dev/.well-known/agent.json)
- **Stateless Hypothesis Red-Team API (`8-Rule Translational Audit`):** `POST / GET https://api.rare-disease-atlas.workers.dev/api/stress-test`
- **`MyelofibrosisBench-v1` (`30` Ground-Truth Eval Tasks + Stdlib Grader):** [`benchmarks/myelofibrosis_bench.jsonl`](https://rare-disease-atlas.github.io/benchmarks/myelofibrosis_bench.jsonl) · [Hugging Face Hub](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)
- **Molecular & Clinical Parquet Join Tables (`DuckDB` Ready):** `myelofibrosis_gene_signatures`, `jak2_structural_pockets`, `myelofibrosis_clinical_trials` on [Hugging Face Datasets](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)
- **Live Daily Myelofibrosis Bio-Delta Wire (`ClinicalTrials.gov v2` + `PubMed`):** [`/atom.xml`](https://api.rare-disease-atlas.workers.dev/atom.xml) · [`/feeds/bio-delta.json`](https://api.rare-disease-atlas.workers.dev/feeds/bio-delta.json)
- **Open Computational Problems & Citation Verifier:** [`/open-problems.json`](https://rare-disease-atlas.github.io/open-problems.json) · [`/.well-known/x402.json`](https://api.rare-disease-atlas.workers.dev/.well-known/x402.json) · [`/CITATION.cff`](https://rare-disease-atlas.github.io/CITATION.cff)

---

## Repositories
- **[`rare-disease-atlas.github.io`](https://github.com/rare-disease-atlas/rare-disease-atlas.github.io)** — Static web atlas, `MyelofibrosisBench-v1`, molecular JSONL tables, `llms-full.txt`, and `/open-problems.json`.
- **[`orphan-disease-opportunity-mcp`](https://github.com/rare-disease-atlas/orphan-disease-opportunity-mcp)** — Zero-dependency Python `stdio` + `.mcpb` MCP server with cryptographic Sigstore SLSA build provenance.
- **[`orphan-disease-venture-scout-skill`](https://github.com/rare-disease-atlas/orphan-disease-venture-scout-skill)** — Portable `SKILL.md` workflow for Claude Code, Cursor, Codex, and autonomous research agents.
