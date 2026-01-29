# SentinelAI – LangChain RAG + Search Agent

SentinelAI is my first AI agent built using LangChain.  
It combines **Retrieval-Augmented Generation (RAG)** with **web search (Tavily)** to answer user queries using both private knowledge and live internet data.

---

## Features

- AI agent architecture using LangChain
- Retrieval-Augmented Generation (RAG)
- Web search using Tavily
- Multi-tool reasoning
- Fallback-safe execution
- Notebook-based experimentation

---

## Tech Stack

- Python 3.10+
- LangChain
- FAISS
- Sentence Transformers
- Tavily Search API
- Groq LLM
- Jupyter Notebook

---

## Project Structure

```
sentinel-ai-agent/
├── notebooks/
│   └── build_agent_legacy.ipynb
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/sentinel-ai-agent.git
cd sentinel-ai-agent
```

---

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate:

**Windows**
```bash
venv\Scripts\activate
```

**Linux / macOS**
```bash
source venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Configure Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here
```

---

### 5. Run the Agent

```bash
jupyter notebook
```

Open:

```
notebooks/build_agent_legacy.ipynb
```

---

## How the Agent Works

1. User submits a query
2. Agent decides whether to:
   - Use RAG (local knowledge)
   - Use Tavily search (web)
3. Relevant context is gathered
4. LLM generates a grounded response
5. Final answer is returned with reasoning

---

## Notes

- `.env` is not committed for security
- The notebook represents the **first working version**
- Code will be modularized in future versions

---

## Author

**Abdullah**  
Senior AI Application Developer  

Focus:
- AI Agents
- RAG Systems
- LLM Applications
- Edge AI

---

## License

MIT License
