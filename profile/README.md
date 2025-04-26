
<!-- README.md for the BioContext GitHub organisation -->

# BioContext

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Docs](https://img.shields.io/badge/docs-online-success)](https://biocontext.ai/docs)
[![Build](https://github.com/BioContext/.github/actions/workflows/ci.yaml/badge.svg)](https://github.com/BioContext/.github/actions)
![SemVer](https://img.shields.io/badge/semver-2.0.0-blue)

> **Enabling AI to speak the language of biology.**  
> BioContext gathers Biomedical Model-Context-Protocol (MCP) **servers** and **agents** in a modular, interoperable ecosystem.

---

## 🌐 What is BioContext?

BioContext is a **collection of open-source MCP servers** that wrap dozens of biology & bio-medicine data APIs—plus reusable agents that let LLMs query them with minimal glue-code.  
The goal is to remove repetitive plumbing so data scientists can focus on **reasoning over knowledge**, not wiring endpoints.

---

## 🧩 Module Index

| Status | Module | Upstream API | Repository | Notes |
|--------|--------|--------------|------------|-------|
| ✅     | `mcp-clinicaltrials` | ClinicalTrials.gov | [`BioContext/clinicaltrials-mcp`](https://github.com/BioContext/clinicaltrials-mcp) | Search & study-detail endpoints |
| ✅     | `mcp-pubchem` | PubChem PUG-REST | [`BioContext/pubchem-mcp`](https://github.com/BioContext/pubchem-mcp) | Compound → synonyms, 2-D/3-D fetch |
| ✅     | `mcp-chembl` | ChEMBL | [`BioContext/chembl-mcp`](https://github.com/BioContext/chembl-mcp) | Bioactivity & target queries |
| 🏗️     | `mcp-openfda` | openFDA / FAERS | [`BioContext/openfda-mcp`](https://github.com/BioContext/openfda-mcp) | Adverse-event & label search |
| 🏗️     | `mcp-rxnorm` | RxNorm | *(planned)* | Drug-concept normalization |
| 🏗️     | `mcp-disgenet` | DisGeNET | *(planned)* | Gene–disease associations |
| 🏗️     | `mcp-stringdb` | STRING | *(planned)* | Protein–protein interactions |
| 🏗️     | `mcp-gnomad` | gnomAD GraphQL | *(planned)* | Variant population frequencies |
| …      | *more coming* | | | |

> **Legend**  ✅ = released & versioned   🏗️ = in active development
