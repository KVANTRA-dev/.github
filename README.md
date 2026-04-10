# KVANTRA

Building tools for knowledge base organization.

---

## What I'm working on

**[NOUZ](https://github.com/KVANTRA-dev/NOUZ-MCP)** — an MCP server for Obsidian that turns a vault into a structured knowledge graph.

The core idea: instead of organizing notes into folders manually, the system classifies them by semantic content and builds a directed acyclic graph (DAG) from the relationships you define. Classification uses cosine similarity against user-defined semantic cores — knowledge domains described as dense embedding texts.

Two things happen simultaneously:

**Top-down** — intent. You define a sign at the top level; it propagates down through structural (hierarchy) links. The human sets the frame.

**Bottom-up** — reality. Atomic notes (quants) get classified by content embeddings. Their domain distribution rolls up as `core_mix`. When intent diverges from reality — the system surfaces `core_drift`. Not an error. A signal.

Semantic bridges are proposed automatically when two notes from different domains have unexpectedly close embeddings. The system finds connections you didn't notice.

Three modes — from pure graph structure (no embeddings needed) to full semantic classification with strict hierarchy validation.

Everything runs locally. No cloud, no telemetry.

---

## Principles

- Structure emerges from content, not from folder names
- Human sets intent, algorithm checks reality
- A note can belong to multiple domains — sign is a spectrum
- Suggestions are proposals. Human decides.

---

## Projects

| | |
|---|---|
| **[NOUZ-MCP](https://github.com/KVANTRA-dev/NOUZ-MCP)** | MCP server for Obsidian. Three modes: pure graph, full semantics, strict hierarchy |
