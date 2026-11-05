# Akshaj Srirambhatla

**Software Engineer · Backend Systems × Applied AI**

B.S. Computer Engineering @ Cal Poly SLO · Software Engineer, AI agents @ Western Digital

I build AI systems that are measured, grounded, and actually deployed.

[Portfolio](https://akshaj01.github.io) · [LinkedIn](https://www.linkedin.com/in/akshaj-srirambhatla/)

---

## Featured: [SEC GraphRAG](https://github.com/Akshaj01/sec-graph-rag)

**Question answering over SEC 10-K filings that cites its sources and is checked against a benchmark.** It combines a Neo4j knowledge graph with pgvector search over the same chunks. A router sends each question to the graph, to vector search, or to both. Answers may cite only chunks from that retrieval.

<p align="center">
  <img src="https://github.com/Akshaj01/sec-graph-rag/raw/main/docs/images/neo4j-graph.png" alt="Neo4j: Apple PRODUCES_PRODUCT edges extracted from the 10-K" width="48%" />
  <img src="https://github.com/Akshaj01/sec-graph-rag/raw/main/docs/images/neo4j-risks.png" alt="Neo4j: Apple EXPOSED_TO_RISK edges extracted from the 10-K" width="48%" />
</p>

- **Grounded by construction:** a closed ontology (6 entity and 8 relationship types), Cypher only from allowlisted templates and never written by the model, and every citation checked against that retrieval's chunk allowlist.
- **10 companies:** AAPL, AMZN, GOOGL, JNJ, JPM, META, MSFT, NFLX, NVDA, XOM. Writes are scoped to the issuer, so one company's filing can't add edges to another company.
- **Measured, not demoed:** 44 hop-stratified questions. Retrieval is scored separately from the answers. An LLM judge is calibrated against hand labels (held-out weighted κ **0.84**). A paired bootstrap compares hybrid with vector-only, and CI fails if hybrid recall@10 regresses.

| 44 questions, 10 companies | Hybrid | Vector-only |
|---|--:|--:|
| Answer score (LLM judge) | **0.92** | 0.89 |
| Out-of-scope questions correctly refused | **12 / 12** | **12 / 12** |
| Retrieval recall@10 | 0.80 | **0.93** |

On this suite the hybrid lead is **not** statistically stable: the 95% CI on the gap runs from −0.05 to +0.13. Vector search also finds the gold passage more often. The repo publishes both results, plus the [five questions it still misses](https://github.com/Akshaj01/sec-graph-rag#what-didnt-work) and a [log of bugs and fixes](https://github.com/Akshaj01/sec-graph-rag/blob/main/docs/PROBLEMS_AND_FIXES.md).

`Python` · `Neo4j` · `pgvector` · `Claude + Instructor` · `OpenAI embeddings` · `FastAPI` · `Docker` · `GitHub Actions`

---

## Other work

| Project | What it is | Stack |
|---|---|---|
| **WD Internal AI Agent** *(Western Digital, internal)* | Python MCP server that turns the MySQL Electrical Failure Analysis database into generated FA reports inside the company's internal AI assistant. Deployed to AWS EKS staging. | Python · MCP · MySQL · AWS EKS |

---

## Tech stack

- **Languages:** Python · C++ · Java · TypeScript · SQL
- **Backend & infra:** FastAPI · Docker · Kubernetes · AWS · MySQL · PostgreSQL
- **AI / data:** RAG · knowledge graphs (Neo4j) · pgvector · MCP · LLM evaluation

---

## Background

Software engineer who started in embedded systems and now builds backend and applied AI systems. Previously a Software Engineer Intern at Toyota North America.

📫 [LinkedIn](https://www.linkedin.com/in/akshaj-srirambhatla/) · [Portfolio](https://akshaj01.github.io)
