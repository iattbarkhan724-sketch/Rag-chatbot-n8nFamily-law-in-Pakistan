Overview

This project is a Retrieval-Augmented Generation (RAG) based chatbot built using n8n, designed to assist users with queries related to Family Law in Pakistan.
It retrieves accurate legal information from law documents and court references, then generates AI-powered responses using the integrated chat model.
Workflow Summary

The workflow is built in n8n and includes the following core components:

Trigger Node (Chat/Manual Trigger) – Starts the chatbot session.

Google Drive Node – Loads PDF files containing Family Law acts, rules, and judgments.

Embedding Model Node – Converts text from PDFs into vector embeddings.

Database Node (Supabase / Vector Store) – Stores the embeddings for retrieval.

RAG Retrieval Node – Fetches the most relevant legal context based on user queries.

Chat Model Node (OpenAI ) – Generates human-like, context-aware answers.

Memory Node – Maintains conversation history for a natural chat experience.
