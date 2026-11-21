# Rare Disease Venture Atlas

[![Live Atlas](https://img.shields.io/badge/Web_Atlas-rare--disease--atlas.github.io-0f766e)](https://rare-disease-atlas.github.io/)
[![RareTxBench v2.0](https://img.shields.io/badge/RareTxBench-v2.0_(152_Test_+_10_Dev_%C2%B7_7_HF_Configs)-9f1d20)](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html)
[![HF RareTxBench](https://img.shields.io/badge/HF_Dataset-RareTxBench-f59e0b)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench)
[![MyelofibrosisBench v1.1](https://img.shields.io/badge/MyelofibrosisBench-v1.1_(50_Test_+_5_Dev)-dc2626)](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html)
[![Remote MCP](https://img.shields.io/badge/MCP_2026--07--28-api.rare--disease--atlas.workers.dev%2Fmcp-0284c7)](https://api.rare-disease-atlas.workers.dev/mcp)
[![VerifyMCP](https://img.shields.io/badge/VerifyMCP-SLSA_Attested-16a34a)](https://verifymcp.io/servers/rare-disease-atlas-orphan-disease-opportunity-mcp/api)
[![Glama](https://img.shields.io/badge/Glama-Grade_A-7c3aed)](https://glama.ai/mcp/servers/rare-disease-atlas/orphan-disease-opportunity-mcp)

An open, citation-backed translational biology & venture opportunity ecosystem built natively for **AI research agents (`RareTxBench-v2.0`, `MyelofibrosisBench-v1.1`, `MCP`, `A2A`, `Parquet`, `Atom`, `x402 $0 Public Good`)** and technical founders—anchored on **Two Paired Flagship Myelofibrosis Deep-Dives** plus frontier-breaking post-diagnosis translational agent benchmarking and live federated diligence across **7,000+ orphan indications**.

---

## Flagship Benchmark: `RareTxBench-v2.0` — 5-Suite Post-Diagnosis Rare-Disease Agent Benchmark (`152` Test + `10` Dev · `7` HF Configs)

Existing rare-disease LLM benchmarks (`RareBench`, `RareArena`) evaluate *phenotype-to-diagnosis* recall, and static MCQs rapidly saturate on frontier reasoning models. **`RareTxBench-v2.0`** breaks frontier saturation across **5 complementary post-diagnosis translational suites (`152` test + `10` dev across `7` Hugging Face configs: `all`, `myelofibrosis`, `cross_orphan`, `open_frontier`, `raw_bio_compute`, `protocol_audit`, `bio_delta_live`)**:

- **Track 1 — `raw_bio_compute` (`12` tasks: `5` MF / `7` Cross-Orphan):** Real RCSB PDB crystal extracts (`4FVR`, `4FVQ`, `5MO4`) + 9 deterministic patient CSV/TSV datasets. Static Frontier Reasoning collapses to **`0.0%` (`100%` CTER)** vs. **`100.0%`** for a code-executing agent.
- **Track 2 — `bio_delta_live` (`10` tasks: `5` MF / `5` Cross-Orphan):** Rolling temporal forensics harvested live (`2026-11-21`) from `ClinicalTrials.gov v2` & late-2026 `PubMed` (`PMID:43061186`, `42980647`, `42663301`, `42849489`, `NCT06343805`, `NCT06313593`, `NCT06128629`). Static Frontier Reasoning scores **`20.0%` (`0.0%` on Myelofibrosis)** vs. **`100.0%`** for a live MCP/API-grounded agent.
- **Track 3 — `protocol_audit` (`10` dense ~500-word Phase 2/3 protocols, `2` clean 0-flaw controls):** Unannounced multi-flaw detection across a 16-code taxonomy. Clean monotonic frontier separation: Lightweight **`30.0%` EM (`79.0%` F1, `34.8%` FN-CTER)** → Standard **`80.0%` EM (`95.7%` F1, `4.4%` FN-CTER)** → Frontier **`90.0%` EM (`97.9%` F1, `0.0%` FN-CTER)**, all with **`0.0%` Clean-Control FP**.
- **Track 4 — `open_frontier` (`20` choice-free exact derivations: `8` MF / `12` Cross-Orphan):** Exposes the **`-65 pt` Recognition–Execution Chasm** (Lightweight `100%` MCQ → `35.0%` open / `50.0%` CTER; Reasoning `100%`).
- **Track 5 — `all` (`100` 6-choice `A–F` MCQ + `10` dev: `40` MF / `60` Cross-Orphan):** `50` `critical_harm` `CTER` safety traps with strict anti-gaming length parity (`Longest-Option = 17.0%` vs `16.7%` random chance).
- **Links:** [Interactive Hub, 5-Q CTER Quiz & Live v2.0 Leaderboard](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html) · [HF Dataset (`rare-disease-atlas/RareTxBench`, 7 Configs)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench) · [GitHub Harness (`rare-tx-bench`: PDB/CSV Artifacts, `lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/rare-tx-bench) · [Live JSON Standings (`/api/rare-tx-leaderboard.json`)](https://api.rare-disease-atlas.workers.dev/api/rare-tx-leaderboard.json)

---

## Paired Flagship Focus: Myelofibrosis (`JAK2+` Clonal vs. Reversible Autoimmune MF)

| Flagship Cohort | Core Biological Wedge | Key Clinical & Genomic Anchors |
| :--- | :--- | :--- |
| **1. Clonal `JAK2 V617F+` Primary Myelofibrosis (`ORPHA:824`)** | Mutant-selective `JH2` pseudokinase allostery (`PDB 4FVQ`/`4FVR`) vs. pan-`JAK1/2` `JH1` cytopenias; Type II persistence breaking; mutant `CALR` biologics; AI marrow fibrosis endpoints | `INCB160058` (`NCT06313593`), `AJ1-11095` (`NCT06343805`), `INCA033989` (`NCT06034002`), `GSE144568`, `GSE156644` |
| **2. Reversible `JAK2`-Negative Autoimmune Myelofibrosis (`AIMF`)** | *"Nature's Positive Control"* proving **74–80% human marrow fibrosis resolution** (`MF-2/3 -> MF-0/1`) on targeted B/T-cell immunomodulation + dual transfusional / `IL-6 -> STAT3 -> hepcidin -> ferroportin` iron overload | Prevents catastrophic `JAK` inhibitor / `HSCT` misrouting in `JAK2`/`CALR`/`MPL` triple-negative & `SLE-AIMF` (`PMID:43061186`) patients |

---

## Open Agent Nectar Suite (`$0` Public Good · Zero Auth Required)

- **`RareTxBench-v2.0` (`152` Test + `10` Dev · `7` HF Configs · `5` Suites):** [Interactive Hub & 5-Q CTER Quiz](https://rare-disease-atlas.github.io/benchmarks/rare-tx-bench.html) · [HF Dataset (7 Configs)](https://huggingface.co/datasets/rare-disease-atlas/RareTxBench) · [GitHub Harnesses & PDB/CSV Artifacts](https://github.com/rare-disease-atlas/rare-tx-bench) · [`GET /api/rare-tx-leaderboard.json`](https://api.rare-disease-atlas.workers.dev/api/rare-tx-leaderboard.json) · 6-Mode Stateless Grader `GET/POST https://api.rare-disease-atlas.workers.dev/api/grade-benchmark` (`rare-tx-raw-bio`, `rare-tx-protocol-audit`, `rare-tx-bio-delta`, `rare-tx-bench-open`, `rare-tx-bench`, `myelofibrosis-bench`)
- **`MyelofibrosisBench-v1.1` (`50` Test + `5` Dev Flagship Eval Tasks):** [Interactive Leaderboard & Mini-Quiz](https://rare-disease-atlas.github.io/benchmarks/leaderboard.html) · [Dedicated HF Dataset](https://huggingface.co/datasets/rare-disease-atlas/MyelofibrosisBench) · [GitHub Harnesses (`lm-eval`, `Inspect AI`, `Promptfoo`)](https://github.com/rare-disease-atlas/myelofibrosis-bench) · [`GET /api/leaderboard.json`](https://api.rare-disease-atlas.workers.dev/api/leaderboard.json)
- **Remote Streamable HTTP MCP (`2026-07-28` & `2025-11-25`):** `https://api.rare-disease-atlas.workers.dev/mcp`
- **Agent2Agent (`A2A v0.3`) Oracle:** `https://api.rare-disease-atlas.workers.dev/a2a` · [`/.well-known/agent.json`](https://api.rare-disease-atlas.workers.dev/.well-known/agent.json)
- **Stateless Hypothesis Red-Team & Molecular Micro-APIs:** `POST /api/stress-test` · `GET /api/gene?symbol=HAMP` · `GET /api/pocket?pdb=4FVQ` · `GET /api/compare?a=jak2-myelofibrosis&b=autoimmune-myelofibrosis`
- **Molecular & Clinical Parquet Join Tables (`DuckDB` Ready):** `myelofibrosis_gene_signatures`, `jak2_structural_pockets`, `myelofibrosis_clinical_trials` on [Hugging Face Datasets](https://huggingface.co/datasets/rare-disease-atlas/rare-disease-venture-atlas)
- **Live Myelofibrosis Bio-Delta Wire & Catalyst Calendar:** [`/atom.xml`](https://api.rare-disease-atlas.workers.dev/atom.xml) · [`/feeds/bio-delta.json`](https://api.rare-disease-atlas.workers.dev/feeds/bio-delta.json) · [`/feeds/catalysts.json`](https://api.rare-disease-atlas.workers.dev/feeds/catalysts.json) · [`/feeds/myelofibrosis-catalysts.ics`](https://api.rare-disease-atlas.workers.dev/feeds/myelofibrosis-catalysts.ics)
- **Open Computational Problems & Citation Verifier:** [`/open-problems.json`](https://rare-disease-atlas.github.io/open-problems.json) · [`/.well-known/x402.json`](https://api.rare-disease-atlas.workers.dev/.well-known/x402.json) · [`/CITATION.cff`](https://rare-disease-atlas.github.io/CITATION.cff)

---

## Repositories
- **[`rare-tx-bench`](https://github.com/rare-disease-atlas/rare-tx-bench)** — `RareTxBench-v2.0` (`152` test + `10` dev across `7` HF configs: `raw_bio_compute`, `bio_delta_live`, `protocol_audit`, `open_frontier`, `MCQ-100`) with real PDB/CSV artifacts and `lm-eval`, `Inspect AI`, and `Promptfoo` harnesses.
- **[`myelofibrosis-bench`](https://github.com/rare-disease-atlas/myelofibrosis-bench)** — `MyelofibrosisBench-v1.1` (`50` test + `5` dev) anchoring the Myelofibrosis/AIMF flagship track inside `RareTxBench-v2.0`.
- **[`rare-disease-atlas.github.io`](https://github.com/rare-disease-atlas/rare-disease-atlas.github.io)** — Static web atlas, interactive `RareTxBench-v2.0` & `MyelofibrosisBench-v1.1` hubs, molecular JSONL tables, `llms-full.txt`, and `/open-problems.json`.
- **[`orphan-disease-opportunity-mcp`](https://github.com/rare-disease-atlas/orphan-disease-opportunity-mcp)** — Zero-dependency Python `stdio` + `.mcpb` MCP server with cryptographic Sigstore SLSA build provenance.
- **[`orphan-disease-venture-scout-skill`](https://github.com/rare-disease-atlas/orphan-disease-venture-scout-skill)** — Portable `SKILL.md` workflow for Claude Code, Cursor, Codex, and autonomous research agents.
