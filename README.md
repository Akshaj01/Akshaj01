# Akshaj Srirambhatla

**Software Engineer · Backend Systems × Applied AI**

B.S. Computer Engineering @ Cal Poly SLO · Software Engineer, AI agents @ Western Digital

I build AI systems that are measured, grounded, and actually deployed.

**Portfolio:** [akshaj01.github.io](https://akshaj01.github.io)

---

## Selected work

| Project | What it is | Stack |
|---|---|---|
| **WD Internal AI Agent** *(Western Digital, internal)* | Python MCP server that turns the MySQL Electrical Failure Analysis database into generated FA reports inside the company's internal AI assistant. Deployed to AWS EKS staging. | Python · MCP · MySQL · AWS EKS |
| **[SEC GraphRAG](https://github.com/Akshaj01/sec-graph-rag)** | Hybrid knowledge-graph (Neo4j) + vector (pgvector) RAG over SEC 10-Ks: closed ontology, no model-written Cypher, citation-validated answers, cost-gated corpus growth. On 44 hop-stratified questions across 10 companies, one temperature-0 run after hybrid-improve fixes: hybrid **0.90** vs vector-only **0.87** (paired gap **+0.026**). Hop-2 hybrid **1.00**. Retrieval: both systems recall@5 **0.84** / MRR **0.70**; vector still leads recall@10 (**0.94** vs **0.91**). Judge held-out κ **0.84**. | Python · Neo4j · pgvector · FastAPI · Docker |
| **[Subby](https://github.com/Akshaj01/subby)** *(work in progress)* | Premiere Pro panel for designing animated subtitles: transcribes a sequence and lays down styled "line boil" subtitle clips I can tweak one by one. Built for my own YouTube videos; a library of After Effects templates to pick from is next. | JavaScript · Adobe UXP · After Effects |

---

## Tech stack

**Languages:** Python · C++ · Java · TypeScript · SQL

**Backend & infra:** FastAPI · Docker · Kubernetes · AWS · MySQL · PostgreSQL

**AI / data:** RAG · knowledge graphs (Neo4j) · pgvector · MCP · LLM evaluation

---

## Background

Software engineer who started in embedded systems and now builds backend and applied AI systems. Previously a Software Engineer Intern at Toyota North America.

📫 [LinkedIn](https://www.linkedin.com/in/akshaj-srirambhatla/) · [Portfolio](https://akshaj01.github.io)
