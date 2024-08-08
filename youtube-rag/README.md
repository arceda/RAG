# Building a RAG application from scratch

This is a step-by-step guide to building a simple RAG (Retrieval-Augmented Generation) application using Pinecone and OpenAI's API. The application will allow you to ask questions about any YouTube video.

## Setup

1. Install
```bash
conda install conda-forge::openai
conda install langchain -c conda-forge
conda install conda-forge::pydantic
conda install conda-forge::pytube
conda install conda-forge::python-dotenv
conda install conda-forge::tiktoken
python -m pip install docarray
python -m pip install -U scikit-learn
python -m pip install pinecone-client
python -m pip install langchain-openai
python -m pip install -U langchain-pinecone
python -m pip install langchain-community langchain-core
python -m pip install ruff
python -m pip install git+https://github.com/openai/whisper.git
```

2. Create a free Pinecone account and get your API key from [here](https://www.pinecone.io/).

3. Create a `.env` file with the following variables:

```bash
OPENAI_API_KEY = [ENTER YOUR OPENAI API KEY HERE]
PINECONE_API_KEY = [ENTER YOUR PINECONE API KEY HERE]
PINECONE_API_ENV = [ENTER YOUR PINECONE API ENVIRONMENT HERE]
```
