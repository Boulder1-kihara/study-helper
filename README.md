# Deep Intel Study Agent: Agentic RAG Pipeline

A lightweight, local-first Agentic Retrieval-Augmented Generation (RAG) pipeline designed to help students study efficiently. Built with LangGraph and Gemini 2.5 Flash, this agent acts as a smart tutor. It first searches your local university notes for answers and autonomously falls back to the web if the local data is insufficient.

## 🚀 Features

* **Agentic Reasoning:** Uses a LangGraph ReAct agent to decide *when* to search local files and *when* to search the internet.
* **Local-First Vector Database:** Keeps heavy document storage local using ChromaDB, ensuring privacy and saving cloud compute costs.
* **Smart Fallback:** Integrates DuckDuckGo API to automatically search the web if past paper questions require external context.
* **Bring Your Own Key (BYOK):** Securely designed so users can input their own Google Gemini API key without hardcoding credentials.
* **Markdown Rendering:** Outputs clean, formatted text, tables, and bullet points directly in Jupyter/Colab notebooks.

## 🛠️ Tech Stack

* **Orchestration:** [LangChain](https://python.langchain.com/) / [LangGraph](https://langchain-ai.github.io/langgraph/)
* **LLM:** Google Gemini 2.5 Flash (`langchain-google-genai`)
* **Vector Store:** ChromaDB (`langchain-chroma`)
* **Embeddings:** HuggingFace `all-MiniLM-L6-v2` (`langchain-huggingface`)
* **Web Search:** DuckDuckGo (`duckduckgo-search`)
* **Document Parsing:** PyPDF (`pypdf`)


## 📦 Installation & Setup

**1. Clone the repository**
```bash
git clone https://github.com/Boulder1-kihara/study-helper.git
cd study-helper




