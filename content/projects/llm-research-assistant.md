---
title: "LLM Research Assistant"
date: 2026-01-10
tags: ["llm", "rag", "typescript"]
description: "A RAG-powered research tool that ingests papers, builds a knowledge graph, and answers complex multi-hop questions."
---

## Overview

Academic research requires synthesizing knowledge across dozens of papers.
This tool ingests research papers, builds a semantic knowledge graph,
and answers complex questions that require reasoning across multiple sources.

## Architecture

- **Document Ingestion:** PDF parsing with layout-aware chunking
- **Knowledge Graph:** Entities and relationships extracted via LLM
- **Hybrid Retrieval:** Dense embeddings + graph traversal for multi-hop queries
- **Answer Synthesis:** Grounded responses with inline citations

## Key Features

- Supports **multi-hop reasoning** across papers
- **Citation tracking** — every claim links back to source material
- **Conversational memory** — follows up on previous questions
- **Export:** Generate literature review drafts from conversation

## Stack

TypeScript, Next.js, Claude API, Pinecone, Neo4j

## What I Learned

RAG is easy to demo, hard to make reliable. The difference between
a toy and a tool is in the retrieval quality — and that comes down
to how you chunk, embed, and rank.
