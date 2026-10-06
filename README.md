# Clinical Trials Intelligence Agent

An AI agent that answers questions about clinical trials and published evidence
for a chosen therapeutic area, combining retrieval over PubMed abstracts with
live queries to ClinicalTrials.gov. Answers include source citations.

> **Status:** Work in progress (v1: basic RAG)
> Built with public data only.

## Problem
Teams in life sciences spend significant time tracking trials and literature
across multiple sources. This project explores how far a well-evaluated
RAG/agent system can automate that workflow.

## Scope
- Therapeutic area: [e.g., GLP-1 therapies in obesity]
- Sources: PubMed abstracts, ClinicalTrials.gov
- Out of scope: [patient data, medical advice, etc.]

## Architecture
_Diagram coming soon._

## Versions and Results
| Version | What changed | Recall@5 | Answer faithfulness | Avg latency | Cost/query |
|---|---|---|---|---|---|
| v1 | Basic vector RAG | - | - | - | - |
| v2 | + Hybrid search, reranking, metadata filters | - | - | - | - |
| v3 | + Agent with tool routing | - | - | - | - |

Evaluation set: [N] hand-written questions in `eval/questions.jsonl`.

## Setup
```bash
git clone <repo-url> && cd clinical-trials-agent
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env   # add your keys
```

## Usage
_Coming soon._

## Limitations
_To be filled in honestly as I learn them._

## Data and Disclaimer
Uses publicly available data from PubMed and ClinicalTrials.gov. This is a
portfolio project and does not provide medical advice.
