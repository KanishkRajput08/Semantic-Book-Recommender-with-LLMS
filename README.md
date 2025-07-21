# SEMANTIC BOOK RECOMMENDER WITH LLMS

This repo contains all of the code to build a Semantic Book Recommender with LLMs.

There are five components:

- **Text data cleaning** (`data-exploration.ipynb`)
- **Semantic (vector) search and building a vector database** (`vector-search.ipynb`). This allows users to find the most similar books to a natural language query (e.g., "a book about a person seeking revenge").
- **Text classification using zero-shot classification in LLMs** (`text-classification.ipynb`). This allows books to be classified as "fiction" or "non-fiction", enabling users to filter books by this facet.
- **Sentiment analysis and emotion extraction using LLMs** (`sentiment-analysis.ipynb`). This allows users to sort books by their tone, such as suspenseful, joyful, or sad.
- **Web application using Gradio** (`gradio-dashboard.py`) for users to get book recommendations.

This project was initially created in Python 3.12.

**Dependencies required:**

- kagglehub
- pandas
- matplotlib
- seaborn
- python-dotenv
- langchain-community
- langchain-ollama
- langchain-chroma
- transformers
- gradio
- notebook
- ipywidgets

A `requirements.txt` file containing all the project dependencies is provided in this repo.

In order to create your vector database, you'll need to install Ollama, run  
`ollama pull nomic-embed-text`  
in your terminal, and ensure Ollama is running before starting the app.
