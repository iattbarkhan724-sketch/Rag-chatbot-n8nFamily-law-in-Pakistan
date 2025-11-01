Overview

This project is a Retrieval-Augmented Generation (RAG) based chatbot built using n8n, designed to assist users with queries related to Family Law in Pakistan.This chatbot describes the domestic and family relationship and matters involving marriage, divorce,child custudy, inheritance and other domestic affairs according to PAKISTAN CIVIL LAW.
It retrieves accurate legal information from 5 law documents MUSLIM FAMILY LAW OF PAKISTAN,DISSOLUTION OF MUSLIM MARRIAGE ACT 1939, CHILD MARRIAGE RESTRAIT ACT 1929, WEST PPAKISTAN FAMILY COURT ACT 1964,GUARDIAN AND WARD ACT 1890, and court references, then generates AI-powered responses using the integrated chat model.
Workflow Summary

The workflow is built in n8n and includes the following core components:

Trigger Node (Chat/Manual Trigger) – Starts the chatbot session.

Google Drive Node – Loads PDF files containing Family Law acts, rules, and judgments.

Embedding Model Node – Converts text from PDFs into vector embeddings.

Database Node (Supabase / Vector Store) – Stores the embeddings for retrieval.

RAG Retrieval Node – Fetches the most relevant legal context based on user queries.

Chat Model Node (OpenAI ) – Generates human-like, context-aware answers.

Post Grase Memory Node – Maintains conversation history for a natural chat experience.
AI AGENT. Answer the queries of any person regarding FAMILY LAW IN PAKISTAN.
