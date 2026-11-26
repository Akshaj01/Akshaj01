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
| **[SEC GraphRAG](https://github.com/Akshaj01/sec-graph-rag)** · [live demo](https://sec-graph-rag.vercel.app) | Hybrid knowledge-graph (Neo4j) + vector (pgvector) RAG over SEC 10-Ks: closed ontology, allowlisted Cypher only, citation-validated answers. On a 44-question suite (10 companies, three temperature-0 runs), hybrid and vector-only tie: **0.96** vs **0.94**, 95% CI on the gap includes zero. Auditing the eval removed an earlier hop-2 "win": the LLM judge penalized real products newer than its training data, and one company had two years of filings indexed. I fixed both, grounding the judge in cited passages (held-out κ **0.79**) and pinning one 10-K per company. | Python · Neo4j · pgvector · FastAPI · Docker |
| **Gymbo** *(iOS, private repo)* | Native iPhone gym tracker built around a split wheel: each bubble is a day of a workout split (Push, Pull, Legs, or a custom one), and the wheel turns to what's next after every workout. Logs machines by brand, each with its own history; prefills every set from last time so one tap logs it; tracks weekly sets per muscle group against a 10–20 set target. Stored on the phone, so it works offline with no login. Opens with Gymbo, a puppy flexing its bicep. | Swift · SwiftUI · Swift Testing · XcodeGen |
| **[Subby](https://github.com/Akshaj01/subby)** *(work in progress)* | Premiere Pro panel for designing animated subtitles: transcribes a sequence and lays down styled "line boil" subtitle clips I can tweak one by one. Built for my own YouTube videos; a library of After Effects templates to pick from is next. | JavaScript · Adobe UXP · After Effects |

---

## Tech stack

**Languages:** Python · C++ · Java · TypeScript · Swift · SQL

**Backend & infra:** FastAPI · Docker · Kubernetes · AWS · MySQL · PostgreSQL

**AI / data:** RAG · knowledge graphs (Neo4j) · pgvector · MCP · LLM evaluation

---

## Background

Software engineer who started in embedded systems and now builds backend and applied AI systems. Previously a Software Engineer Intern at Toyota North America.

📫 [LinkedIn](https://www.linkedin.com/in/akshaj-srirambhatla/) · [Portfolio](https://akshaj01.github.io)
