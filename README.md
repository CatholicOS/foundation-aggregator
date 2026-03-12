# Catholic Tech Content Aggregator

This repository is a brainstorming area for ideas and approaches on how to build a news, blog, video, podcast, and project aggregator at the intersection of faith and technology for the **Catholic Digital Commons Foundation (CDCF)** website.

## Project Vision

The goal is to create a system that surfaces high-quality content relevant to the Catholic Church and modern technology. We are exploring various architectures and tools to make this process efficient, scalable, and accurate.

## Suggested Approaches

Several approaches are currently being discussed:

### 1. Low-Code / MCP Integration
- **Tools:** n8n, Brave Search API, and Model Context Protocol (MCP).
- **Concept:** Use n8n for orchestration, leveraging the Brave Search API via MCP to pull relevant snippets and content.

### 2. Brave Search API Optimization
- **Concept:** Use the Brave Search API specifically to pull snippets as an optimization step.
- **Benefit:** This can reduce costs and improve efficiency by avoiding full page crawls when snippets provide enough context for initial classification or filtering.

### 3. Autodiscovery & Human-in-the-Loop
- **Concept:** Implement a system that automatically discovers new websites, RSS feeds, and sources.
- **Validation:** These discovered sources are presented to the CDCF team for approval. 
- **Evolution:** As the system's confidence grows based on human feedback, it can eventually transition to a more autonomous mode of operation.

### 4. Detailed Implementation Plan (SQL + Python + Next.js)
For a more structured architectural proposal involving PostgreSQL (with Apache AGE), Python workers, and a Next.js frontend, see [content-aggregator.md](./content-aggregator.md).

## Contributing

This project is open for brainstorming and contributions! If you have ideas on how to improve the aggregation system, simplify the architecture, or integrate better tools, please feel free to:

- Open an issue to discuss a new approach.
- Submit a Pull Request with documentation or proof-of-concept code.
- Join the conversation on how we can best serve the intersection of faith and technology.
