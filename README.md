# RagPipeline
RAG application using Groq which accepts PDF files .

# Code Description

This Markdown file describes a Python script that performs document indexing, retrieval, and generation using various natural language processing (NLP) techniques and libraries.

## Code Overview

The provided Python script performs the following tasks:

1. **Importing Libraries**: The script imports several libraries necessary for document processing, including BeautifulSoup (`bs4`), `langchain`, `RecursiveCharacterTextSplitter`, `WebBaseLoader`, `Chroma`, `StrOutputParser`, `RunnablePassthrough`, `ChatGroq`, `HuggingFaceEmbeddings`, and `TextLoader`.

2. **Indexing Phase**:
   - It loads a PDF document using `PyPDFLoader`.
   - Splits the document into smaller chunks using `RecursiveCharacterTextSplitter`.
   - Creates embeddings for each chunk using `Chroma` and `HuggingFaceEmbeddings`.

3. **Retrieval and Generation Phase**:
   - Defines a retrieval and generation pipeline using `ChatGroq`, `hub`, and other related components.
   - Utilizes a predefined prompt for generating responses based on user queries related to the indexed document.

4. **Question Input**:
   - Invokes the defined pipeline with a user-generated question related to the indexed PDF data.

## Usage

The script can be used to process and interact with PDF documents. After indexing a document, users can ask questions about its content, and the script will generate relevant responses based on the indexed data.

## Important Notes

- Ensure that all necessary libraries are installed before running the script.
- This script provides a basic implementation and may require customization for specific use cases or document formats.

