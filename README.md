# LangSmith Observability with RAG

A simple RAG application built with LangChain, LangSmith, OpenRouter, and Hugging Face embeddings.

This project demonstrates how to build a banking support assistant that retrieves relevant information from documents and generates answers using an LLM. LangSmith is used to trace and observe the RAG workflow.

## Features

* Retrieval-Augmented Generation (RAG)
* Banking customer support Q&A
* Hugging Face embeddings
* In-memory vector store
* OpenRouter LLM
* LangChain prompts and retriever
* LangSmith tracing and observability
* Basic LangGraph agent workflow

## Architecture

```text
User Question
      |
      v
   Retriever
      |
      v
Relevant Documents
      |
      v
    Context
      |
      v
   LLM
      |
      v
 Final Answer
      |
      v
 LangSmith
  Tracing
```

## Technologies

* Python
* LangChain
* LangGraph
* LangSmith
* OpenRouter
* Hugging Face
* InMemoryVectorStore
* Jupyter Notebook

## Project Structure

```text
LangSmith-Observability/
│
├── observability.ipynb
├── .env.example
├── .gitignore
├── pyproject.toml
└── README.md
```

## Setup

Clone the repository:

```bash
git clone https://github.com/iam-k7/LangSmith-Observability.git
cd LangSmith-Observability
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

If you are using `pyproject.toml`, install the project with:

```bash
pip install -e .
```

## Environment Variables

Create a `.env` file in the project root:

```env
LANGSMITH_API_KEY=your_langsmith_api_key
OPENROUTER_API_KEY=your_openrouter_api_key
HF_TOKEN=your_huggingface_token
```

Never commit your `.env` file to GitHub.

Use `.env.example` as a template.

## Run the Project

Open the notebook:

```bash
jupyter notebook observability.ipynb
```

Or open `observability.ipynb` directly in VS Code and run the cells.

## Example Questions

The banking RAG assistant can answer questions such as:

```text
How can I open a new bank account?

How do I report a lost debit card?

How can I check my account balance?

How can I transfer funds?

Can I set up direct deposit?

When is the bank office open?
```

## LangSmith Observability

LangSmith is used to trace the application and monitor the RAG workflow.

The traces can help inspect:

* User questions
* Retrieved documents
* Prompts
* LLM calls
* Generated responses
* Execution flow
* Errors and debugging information

Set the LangSmith environment variables before running the application.

## Security

Do not commit API keys or other sensitive credentials.

The following files should remain local:

```text
.env
.venv/
```

Use `.env.example` for sharing required environment variable names.

## Learning Goals

This project is useful for learning:

* RAG fundamentals
* Vector search
* Embeddings
* LangChain
* LangGraph
* LLM integration
* Prompt engineering
* LangSmith tracing
* AI application observability

## Future Improvements

* Add a persistent vector database
* Add document upload and processing
* Add source citations
* Improve retrieval with reranking
* Add authentication and authorization
* Add evaluation with LangSmith
* Add a web interface
* Deploy the application

## Author

Kesavan

GitHub: https://github.com/iam-k7

## License

This project is for learning and experimentation.
