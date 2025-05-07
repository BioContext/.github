<!-- BioContext README — regenerated 2025-05-07 -->

<p align="center">
  <a href="https://discord.gg/dyArWuje" target="_blank">
    <img src="https://img.shields.io/badge/Join%20our-Discord-5865F2?logo=discord&logoColor=white&style=for-the-badge"
         alt="Discord invite">
  </a>
</p>

# BioContext

> **Enabling AI to speak the language of biology.**  
> BioContext is an open-source collection of Model Context Protocol (MCP) servers that wrap major bio-databases and make them instantly query-able by LLMs and agent frameworks.

---

## Repositories (active)

| Status | Repo | Data Source | Quick blurb | Last update* |
| :---: | --- | --- | --- | --- |
| ✅ | **BioMart-MCP** | [BioMart](https://www.biomart.org) | Query federated genomic datasets via BioMart. | 2025-05-03 |
| ✅ | **PubMed-MCP** | [PubMed](https://pubmed.ncbi.nlm.nih.gov) | Search & retrieve biomedical citations. | 2025-05-01 |
| ✅ | **BioContext-main** | — | Meta-repo & Helm/Docker orchestration for all sub-servers. | 2025-04-21 |
| ✅ | **OpenTargets-MCP** | [Open Targets Platform](https://platform.opentargets.org) | Drug-target evidence & associations. | 2025-04-21 |
| ✅ | **AACT-MCP** | [AACT / ClinicalTrials.gov](https://aact.ctti-clinicaltrials.org) | Access aggregated clinical-trials data. | 2025-04-21 |
| ✅ | **AlphaFold-MCP** | [AlphaFold DB](https://alphafold.ebi.ac.uk) | Retrieve predicted protein structures. | 2025-04-18 |
| ✅ | **UniProt-MCP** | [UniProt](https://www.uniprot.org) | Protein sequences & annotations. | 2025-04-17 |
| ✅ | **ChemBL-MCP** | [ChEMBL](https://www.ebi.ac.uk/chembl) | Bioactivity / drug-like molecules. | 2025-04-17 |
| ✅ | **PubChem-MCP** | [PubChem](https://pubchem.ncbi.nlm.nih.gov) | Compounds, substances & assays. | 2025-04-17 |

\*“Last update” = last push on GitHub at time of this README refresh (7 May 2025).

> Looking for install instructions?  
> Every repo ships its own **README** with `pip`/`uv`/Docker commands and examples.

---

## Why MCP?

MCP is an open specification that lets external tools expose **structured resources**, **tools**, and **prompts** to AI assistants over simple transports (STDIO, HTTP, SSE). Wrapping bio-databases behind MCP servers means:

* **Zero-boilerplate** integration with clients such as Claude Desktop, Cursor IDE, or AutoGen agents.  
* **Schema discovery** – each tool is self-describing via JSON Schema.  
* **Language-agnostic** – works with Python, Node, Go, Rust, … anything that can read/write JSON.

---

## Quick start (one-liner demo)

```bash
# Example: spin up PubChem-MCP in a fresh venv
uv venv && source .venv/bin/activate
pip install pubchem-mcp
pubchem-mcp --stdio   # now point your MCP-aware client at STDIO


