# RAG OpenAI Native

This project implements a Retrieval-Augmented Generation (RAG) pipeline using OpenAI's native APIs and Pinecone for vector storage.

## Features

* PDF document ingestion
* Text chunking with overlap
* OpenAI embeddings (`text-embedding-3-small`)
* Pinecone vector storage
* Semantic retrieval using cosine similarity
* Answer generation with OpenAI Chat Completions
* Source page citations

## Project Structure

```text
lab-rag-openai-native/
│
├── rag_openai_native.ipynb
├── README.md
├── lab_summary.md
├── .env
├── .gitignore
└── data/
```

## How to Run

1. Create a `.env` file containing:

```env
OPENAI_API_KEY=your_key
PINECONE_API_KEY=your_key
```

2. Install dependencies:

```bash
pip install openai numpy python-dotenv pypdf2 tiktoken pinecone
```

3. Open and run:

```text
rag_openai_native.ipynb
```

## Example Questions

* What role did Loose Change play in conspiracy culture?
* What role did David Icke play in conspiracy culture?
* Who won the Premier League in 2025?

The system answers using retrieved document context and includes source page references.
