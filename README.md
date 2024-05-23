# Revelation: Llama_3_RAG

Welcome to the Revelation project! This repository contains the code and resources for the Llama_3_RAG implementation. The goal of this project is to enhance retrieval-augmented generation (RAG) capabilities using the Llama 3 model.

## Table of Contents

- [Introduction](#introduction)
- [Setup](#setup)
- [Usage](#usage)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Introduction

Retrieval-Augmented Generation (RAG) is a technique that combines document retrieval with generative models to produce more accurate and context-aware outputs. This project leverages the Llama 3 model to implement Advanced RAG techniques, namely Adaptive-RAG, SELF-RAG, and Corrective RAG, enhancing its ability to generate accurate and meaningful text based on retrieved documents and web search.

## Setup

To set up the project locally, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/waldemarchang/Revelation.git
    cd Revelation
    ```

2. **Install Ollama**:
    - Type in your terminal:
    ```sh
    curl -fsSL https://ollama.com/install.sh | sh
    ollama serve & ollama pull llama3
    ```

3. **Install the required dependencies**:
    ```sh
    pip install -q -U langchain-nomic langchain_community tiktoken langchainhub chromadb langchain langgraph tavily-python gpt4all pypdf gradio html2text faiss-cpu sentence-transformers
    ```

4. **Additional steps for Google Colab users**:
    - Install `colab-xterm` to open a terminal within Colab:
    ```sh
    pip install -q -U colab-xterm
    ```
    - Load and start `colab-xterm`:
    ```python
    %load_ext colabxterm
    %xterm
    ```
    - Once the terminal opens, you can run the Ollama setup commands within it:
    ```sh
    curl -fsSL https://ollama.com/install.sh | sh
    ollama serve & ollama pull llama3
    ```

## Usage

1. **Open the Jupyter Notebook**:
    ```sh
    jupyter notebook Llama_3_RAG.ipynb
    ```

2. **Run the notebook**:
   - Follow the instructions in the notebook to execute the cells.
   - Ensure you understand each step before running the cell to avoid errors.

## Acknowledgements

This project is based on the work of the authors of the LangGraph project. It was built upon their foundation to enhance retrieval-augmented generation capabilities. Their project can be found here:
[LangGraph Project](https://github.com/langchain-ai/langgraph/blob/main/examples/rag/langgraph_rag_agent_llama3_local.ipynb)

Special thanks to the original authors:

- LangGraph Authors

Their work laid the foundation upon which this project was built to achieve specific goals.

## License

This project is licensed under the MIT License - see the LICENSE file for details.