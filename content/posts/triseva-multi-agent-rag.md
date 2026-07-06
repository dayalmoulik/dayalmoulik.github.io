---
title: "TRISEVA: Multi-Agent RAG System for Cross-Domain Document QA"
date: 2026-07-06
description: "An overview of TRISEVA, a multi-agent Retrieval-Augmented Generation system designed for explainable question answering across Healthcare, Legal/Government, and Agriculture domains."
menu:
  sidebar:
    name: TRISEVA
    identifier: triseva-multi-agent-rag
    weight: 1
---

## Introduction

In the current landscape of Large Language Models (LLMs), retrieving accurate information from domain-specific documents is a major challenge. Standard Retrieval-Augmented Generation (RAG) systems often fail when dealing with complex terminology and structured files across highly diverse sectors like Healthcare, Law, and Agriculture. 

To solve this, I designed **TRISEVA** (a Multi-Agent Retrieval-Augmented System) as part of my M.Tech dissertation at BITS Pilani.

## Architecture

TRISEVA employs a modular multi-agent architecture where specialized agents collaborate to analyze, retrieve, and formulate explainable answers:

1. **Domain Classifier Agent**: Routes user queries to the specific domain context (Healthcare, Legal/Government, or Agriculture).
2. **Retrieval Specialist Agent**: Queries local vector stores optimized for specific terminologies and document hierarchies.
3. **Explainer Agent**: Interprets the retrieved context and structures the output to show source citations and confidence scores, providing transparency.

## Key Technologies Used

- **LangChain & LangGraph**: For defining stateful, collaborative agent graphs.
- **Python**: Core programming language.
- **TensorFlow / PyTorch**: For embedding tuning and text processing.
- **ChromaDB / PGVector**: Used to cache and query semantic embeddings.

## Conclusion

By breaking down the retrieval and reasoning tasks into specialized agents, TRISEVA delivers explainable, highly accurate domain answers, reducing hallucinations significantly and making QA reliable for critical fields.
