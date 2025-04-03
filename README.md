# LexRAG 🧠⚖️

**LexRAG** (Legal Expert Retrieval-Augmented Generation) is an **Agentic RAG system** for real-time monitoring and summarization of sanctions and compliance updates — powered by a quantized LLaMA model, LangChain agents, and real-time data tools.

> Use it to track OFAC/Treasury sanctions, summarize legal developments, or stay ahead of global regulatory actions — with citations and verifiable sources.

---

## 🔍 What It Does

LexRAG answers questions like:

- *"Are there any new OFAC sanctions on North Korea in 2025?"*
- *"Has OFAC released recent updates about Iran or crypto-related activities?"*

It retrieves real-time and official information, then **uses an LLM to synthesize a summary** with proper references.

---

## 🛠️ How It Works

LexRAG is a multi-tool LangChain agent enhanced by:

### 🔗 **Agentic Architecture**
- 🧠 Quantized [`meta-llama/Llama-3.2-3B-Instruct`](https://huggingface.co/meta-llama/Llama-3.2-3B-Instruct) model via `bitsandbytes`
- 🔎 Real-time search with `DuckDuckGoSearch`
- 📡 OFAC/Treasury.gov RSS feed parser
- 📚 Combined context summarized via LLM
- 💬 Agent reasoning using LangChain's ReAct-style executor

---

## 🧱 Tech Stack

| Component     | Role |
|--------------|------|
| 🧠 LLaMA 3.2 3B | Language model for final summarization |
| ⚙️ LangChain  | Agent framework & tool integration |
| 🔍 DuckDuckGoSearch | Real-time web search |
| 📡 Feedparser | Treasury.gov RSS parsing |
| 💨 BitsAndBytes | 4-bit quantized model loading |
| 🐍 Python     | End-to-end implementation |

---

## 🚀 Quickstart

### 1. Clone this repo
```bash
git clone https://github.com/your-username/LexRAG.git
cd LexRAG
