---
layout: page
title: RAG Scientific Paper QA
description: A retrieval-augmented assistant for grounded question answering over scientific papers.
importance: 1
category: applied-ai
github: https://github.com/XINGYI-PU/rag-paper-qa
---

## Overview

This project explores whether retrieval-augmented generation can make answers about scientific papers easier to verify and less dependent on a language model's general knowledge. It uses a small, reproducible sample from the QASPER dataset and compares direct generation with retrieval-grounded generation.

## Technical approach

- Converts papers into overlapping text chunks and embeds them with `BAAI/bge-m3`.
- Builds a FAISS index and retrieves supporting passages with cosine similarity.
- Generates answers with Qwen2.5-7B-Instruct or Mistral-7B-Instruct-v0.3.
- Compares four settings: direct and RAG generation with each model.
- Supports quantitative evaluation, manual scoring, and evidence-hit analysis.
- Provides a Streamlit interface that displays answers, retrieved evidence, and similarity scores.
- Includes a mock mode for lightweight testing without downloading large models.

**Technologies:** Python, Hugging Face Transformers, FAISS, Streamlit, QASPER, Qwen, and Mistral.

[View source code and documentation on GitHub](https://github.com/XINGYI-PU/rag-paper-qa).
