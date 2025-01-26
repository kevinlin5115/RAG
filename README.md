# RAG Pipeline with Neural Grading

A Retrieval-Augmented Generation (RAG) system with neural grading for improved context relevance and response quality.

## Overview

- PGVector containerized and deployed on remote machine
- Local GPU-accelerated embeddings (Nomic AI)
- Context relevance evaluation using LLM
- Question answering with filtered contexts

## Architecture

- BaseEvaluator: Abstract base class for evaluation modules
- RelevanceGrader: Assesses context relevance
- QuestionAnswering: Generates responses using filtered contexts
- HallucinationGrader: Validates answer factual accuracy
- Containerized PostgreSQL/pgvector for scalable vector storage

## Status: Work in Progress

Upcoming features:
- Web search fallback when no relevant local contexts found
- Response caching for improved latency
- Query expansion for better context retrieval
- Additional evaluation metrics