# InsureAI-Smart-Health-Insurance-Assistant_Rag

# DocuSense AI: RAG-Powered Document Intelligence

## Overview
DocuSense AI is a document question-answering project built using Retrieval-Augmented Generation (RAG).
It retrieves relevant information from PDF documents and generates context-based answers using a Large Language Model (LLM).
The project also uses LLM-as-a-Judge to evaluate answer quality.

## Objectives
- Build a document-based question-answering system.
- Retrieve relevant information from PDF documents.
- Generate answers grounded in retrieved context.
- Evaluate answers for groundedness and relevance.
- Compare baseline LLM responses with RAG responses.

## Key Features
- PDF text extraction using PyMuPDF.
- Text chunking with overlapping passages.
- Semantic embeddings using Sentence Transformers.
- Vector storage and similarity search using ChromaDB.
- Context-based answer generation using a local Llama model.
- LLM-as-a-Judge evaluation using a 1–5 scoring scale.
- Comparison of baseline and RAG-generated answers.

## Technologies Used
- Python
- LangChain
- Llama
- ChromaDB
- Sentence Transformers
- Hugging Face
- PyMuPDF
- Jupyter Notebook / Google Colab

## Project Workflow
1. Load and extract text from a PDF document.
2. Split the text into smaller overlapping chunks.
3. Generate semantic embeddings for the chunks.
4. Store embeddings in a Chroma vector database.
5. Retrieve relevant chunks based on the user's question.
6. Provide the retrieved context to the LLM.
7. Generate an answer using the local Llama model.
8. Evaluate groundedness and relevance using an LLM judge.
9. Compare baseline and RAG evaluation results.

## Evaluation Metrics
- **Groundedness:** Measures whether the answer is supported by the retrieved context.
- **Relevance:** Measures whether the answer addresses the user's question.
- Both metrics use a scoring scale from 1 to 5.

## Current Implementation Note
The current notebook demonstrates the RAG workflow using an Apple innovation article.
To adapt the project for health insurance, use authoritative insurance policy PDFs and validate answers about coverage, exclusions, waiting periods, eligibility, and claims.

## Limitations
- Answer quality depends on document quality and retrieval accuracy.
- LLM-as-a-Judge may produce incorrect evaluations.
- The sample evaluation does not guarantee performance on other documents.
- Human review is necessary before relying on answers for important decisions.

## Future Improvements
- Add source citations and page numbers to answers.
- Develop an interactive PDF question-answering interface.
- Evaluate performance using more test questions.
- Compare different embedding models and chunking strategies.
- Introduce human feedback and additional evaluation methods.

## Author
**Name:** Your Name  
**GitHub:** Your GitHub Profile URL  
**LinkedIn:** Your LinkedIn Profile URL
