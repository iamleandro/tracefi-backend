# 🔎 TraceFi Backend

**TraceFi** is an open-source blockchain OSINT platform that helps users trace cryptocurrency wallet activity, identify connections between addresses, and follow the flow of funds on public ledgers like Ethereum and Bitcoin.

This repository contains the FastAPI-based backend that handles:
- Wallet metadata retrieval
- Transaction parsing
- Relationship graph building
- OSINT enrichment modules (coming soon)

---

## 🛠️ Tech Stack

- Python 3.11
- [FastAPI](https://fastapi.tiangolo.com/)
- NetworkX (for graph analysis)
- Etherscan / BlockCypher API (wallet data)
- SQLite (default database)
- Docker (optional)

---

## 🚀 Getting Started

### 🔧 Requirements

- Python 3.10+
- `pip` / `venv`
- Docker (optional, but recommended)

---

### 🧱 Local Setup (no Docker)

```bash
git clone https://github.com/yourusername/tracefi-backend.git
cd tracefi-backend

python3 -m venv venv
source venv/bin/activate

pip install -r requirements.txt

uvicorn app.main:app --reload
```

Visit http://localhost:8000/docs to explore the API.

---

### 🐳 Local Setup with Docker

```bash
docker build -t tracefi-backend .
docker run -p 8000:8000 tracefi-backend
```

---

### 📌 Coming Soon

- Wallet graph builder (NetworkX)
- Wallet clustering logic
- Enrichment from public sources (ENS, leaks, Reddit)
- Suspicion scoring (ML)