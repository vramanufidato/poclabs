# POC Labs

**Hands-on AI, cloud, and security labs — notebooks, Python apps, and Word lab guides.**

This repository consolidates the lab work I have completed across my AI, cloud, and security learning repositories. It is a working lab book: each folder contains self-contained notebooks or lab guides, and each section README explains what every file does.

**89 lab artifacts · 38.7 MB · 48 notebooks · 38 Word labs · 3 Python scripts**

## Repository map

| Section | Labs | What is inside |
| --- | ---: | --- |
| [Agentic AI](ai-genai/agentic-ai/README.md) | 15 | Agent frameworks, graph workflows, and multi-agent orchestration. |
| [AI Agents](ai-genai/ai-agents/README.md) | 6 | Tool-calling agents, natural-language interfaces, and agentic app patterns. |
| [Multimodal AI](ai-genai/multimodal/README.md) | 7 | Image, audio, and text applications combining multiple model types. |
| [RAG](ai-genai/rag/README.md) | 6 | Retrieval-augmented generation, document QA, and retrieval strategies. |
| [Vector Databases](ai-genai/vector-databases/README.md) | 7 | Embeddings, similarity search, ChromaDB, and FAISS. |
| [Model Context Protocol](ai-genai/mcp/README.md) | 5 | MCP clients, servers, and advanced protocol features. |
| [GCP Data Engineering](cloud-gcp/data-engineering/README.md) | 6 | BigQuery, Vertex AI, Natural Language API, and data pipelines. |
| [GKE](cloud-gcp/gke/README.md) | 2 | Google Kubernetes Engine and BigQuery from JupyterLab. |
| [Security Python](security/python/README.md) | 20 | Python programming activities and exemplars from the security course. |
| [Linux](security/linux/README.md) | 6 | Linux command-line labs for users, files, permissions, and packages. |
| [SQL](security/sql/README.md) | 5 | SQL query, filter, and join labs. |
| [Security Analysis](security/analysis/README.md) | 4 | Packet capture, Wireshark, hashing, and decryption labs. |
| **Total** | **89** | **38.7 MB** |

## How to use

- **Notebooks (`.ipynb`)** — open in Jupyter Lab, VS Code, or Google Colab. Install the packages imported in the first cell; many labs use LangChain, LlamaIndex, CrewAI, AutoGen, ChromaDB, FAISS, or IBM watsonx.
- **Word labs (`.docx`)** — open in Microsoft Word or Google Docs. These contain step-by-step instructions, screenshots, and expected outputs.
- **Python scripts (`.py`)** — application entry points for the Gradio and RAG demos. Review the imports and provide the required model/API configuration before running.
- **Source mapping** — [`manifest.csv`](manifest.csv) lists every file with its original repository path, size, and section.

## Curation notes

- Duplicate `(1)` copies were removed by content hash, so each lab appears once.
- Course reading PDFs, graded-quiz answer documents, Canva instructions, and unrelated business/portfolio documents were intentionally excluded.
- Files are copied as-is from the source repositories. Some notebooks expect local data files, cloud credentials, or API keys that are not included here.
- Do not commit real API keys or cloud credentials. Use environment variables or a local `.env` file excluded by `.gitignore`.

## Source repositories

- `Architect/AI/genai2` — GenAI, agentic AI, RAG, multimodal, vector database, and MCP labs.
- `Architect/Cloud/cloud/gcp` — Google Cloud data engineering and GKE labs.
- `Architect/security` — Python, Linux, SQL, and security-analysis labs.

## Getting started

```bash
cd poclabs
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate

pip install jupyterlab
jupyter lab
```

Open the notebook for the lab you want to run and follow its setup cell. For Word labs, open the `.docx` directly.

---

Maintained by Venkatesh R.
