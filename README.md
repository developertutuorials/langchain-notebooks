# 🦜🔗 LangChain Notebooks

A collection of hands-on Jupyter notebooks for learning **LangChain** — from building chatbots to implementing RAG (Retrieval-Augmented Generation) pipelines.

---

## 📁 Notebooks

### 1. `1-chatbots.ipynb` — Chatbot with Memory
Learn how to build a conversational chatbot using LangChain that remembers past messages.

**Topics Covered:**
- Setting up LLM with LangChain
- Adding chat history / memory
- Building multi-turn conversation chains
- Using `ChatPromptTemplate`

---

### 2. `vectorretriever.ipynb` — Vector Store & RAG Pipeline
Learn how to store documents as vectors and retrieve them intelligently to answer questions.

**Topics Covered:**
- HuggingFace Embeddings (`all-MiniLM-L6-v2`)
- ChromaDB Vector Store
- Building a Retriever using `as_retriever()` and `RunnableLambda`
- RAG Chain using LCEL (`|` operator)
- Conversation Q&A with context

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🦜 LangChain | LLM framework |
| 🤗 HuggingFace | Embeddings model |
| 🟣 ChromaDB | Vector database |
| 🔥 PyTorch | Backend for embeddings |
| 📓 Jupyter | Interactive notebooks |

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/developertutuorials/langchain-notebooks.git
cd langchain-notebooks
```

### 2. Create virtual environment
```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install langchain langchain-core langchain-community
pip install langchain-huggingface chromadb
pip install torch torchvision torchaudio
pip install jupyter
```

### 4. Setup environment variables
Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```

### 5. Run notebooks
```bash
jupyter notebook
```

---

## 📖 Concepts Explained

```
User Query
    │
    ▼
Embeddings Model  ──▶  VectorStore (ChromaDB)
                              │
                              ▼
                         Retriever
                              │
                              ▼
                    Prompt Template + LLM
                              │
                              ▼
                         Final Answer ✅
```

---

## ⚠️ Important Notes

- Never push your `.env` file — it contains API keys
- Restart Jupyter kernel after installing new packages
- `all-MiniLM-L6-v2` model downloads automatically on first run (~90MB)

---

## 📚 Resources

- [LangChain Docs](https://python.langchain.com/)
- [HuggingFace Models](https://huggingface.co/models)
- [ChromaDB Docs](https://docs.trychroma.com/)

---

