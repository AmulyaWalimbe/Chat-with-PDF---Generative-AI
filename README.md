# Chat-with-PDF---Generative-AI

## Project Overview
Our project is a cloud-based “Chat with PDF” application built using Amazon Bedrock, Titan Embeddings, Claude 3 Sonnet, LangChain, Docker, and Amazon S3. The goal is to allow users to ask natural-language questions about a PDF and receive accurate, grounded answers based strictly on the document’s content.

We built two separate interfaces:
  1) Admin Interface that uploads the PDF, extracts the text, generates embeddings, and creates a FAISS vector index stored in Amazon S3, and
  
  2) User Interface that loads this index, runs similarity search using FAISS, and sends the retrieved text to Claude for answer generation.
  
The Project follows the Retrieval-Augmented Generation (RAG) approach, enabling fast, reliable, and secure document querying without exposing or modifying the original PDF.
