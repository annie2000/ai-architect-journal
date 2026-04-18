# 2026-04-18 — Friday (SAMPLE)

**Time spent:** 17 min
**Source type:** Blog

> ⚠️ This is a SAMPLE entry to show what a completed entry looks like. Delete this file or keep it as reference.

---

## Source

[Building effective agents](https://www.anthropic.com/research/building-effective-agents)
— *Published by: Anthropic Research*

## One-Sentence Summary

Anthropic argues that the most effective AI agent architectures are not complex multi-agent frameworks but simple compositions of LLM calls with tools, where complexity is added only when measurably justified.

## Key Concept Explained

**Concept:** The Orchestrator-Workers Pattern

Imagine you're a project manager who receives a vague request: "Prepare our Q3 customer health report." You don't do everything yourself. Instead, you break the task into pieces, assign each piece to a specialist, and then stitch the results together.

The orchestrator-workers pattern works the same way. A central LLM (the orchestrator) receives a complex task, decomposes it into subtasks, and delegates each subtask to a separate LLM call (a worker). Each worker operates independently — it might search a database, analyze a document, or generate a section of text. The orchestrator then synthesizes all the worker outputs into a final response.

What makes this different from a simple chain is that the orchestrator decides dynamically how many workers to spawn and what each one should do. The subtask breakdown isn't hardcoded — it adapts based on the input.

## Connection to My Work

This maps directly to how ServiceNow AI Agent Studio structures multi-step agent workflows. When we build a custom AI Agent with multiple topics, each topic is essentially a "worker" that handles a specific intent. The orchestration layer (Now Assist's ReAct loop) decides which topic to route to based on the user's input. When I explain AI Agent architecture to SI partners like Virtusa, the orchestrator-workers mental model is much more intuitive than jumping straight into ReAct or Chain-of-Thought terminology.

## New Vocabulary

| Term | Definition (in my own words) | Example sentence |
|------|------------------------------|------------------|
| augmented LLM | An LLM enhanced with tool access (search, code execution, etc.) rather than working from memory alone | "Now Assist is an augmented LLM — it doesn't just generate text, it can query the CMDB and trigger workflows." |
| orchestrator-workers | A pattern where one LLM breaks a task into subtasks and delegates each to separate LLM calls | "Our multi-agent demo uses an orchestrator-workers pattern where the triage agent routes to specialized fulfillment agents." |

## Raw Reaction (Optional)

The biggest takeaway for me is the emphasis on starting simple. I've been defaulting to complex multi-agent designs in my enablement materials because they sound impressive. But Anthropic is saying — if a single LLM call with good prompting solves the problem, don't add agents. This changes how I should frame the AI Agent Fabric story to partners. Start with "do you even need agents?" before jumping to MCP/A2A.

