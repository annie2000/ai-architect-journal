# AI Architect Journal

**Daily English technical learning journal — 15 minutes before work, every morning.**

## Why This Exists

This repo is a deliberate practice system for two things at once:
1. **Deep technical fluency** in AI/ML architecture, protocols, and platforms
2. **English technical writing** — thinking and expressing ideas directly in English, not translating from Korean

## The Rules

### Non-Negotiable
- **English only.** No Korean anywhere in this repo. Not even comments.
- **No translation.** Read in English → think in English → write in English.
- **15 minutes max.** Timer on. Stop when it rings. Consistency beats volume.
- **Imperfect is fine.** Grammar mistakes are expected. Don't self-edit for 15 minutes — just write.

### Daily Entry Format
Every entry follows the same structure (see `templates/daily-entry.md`):

```
## Source
[What you read — link + title]

## One-Sentence Summary
[Force yourself to compress the entire piece into ONE sentence]

## Key Concept Explained
[Pick ONE concept and explain it as if teaching a junior SC who's never heard of it]

## Connection to My Work
[How does this relate to ServiceNow, partner enablement, or a customer scenario?]

## New Vocabulary
[2-3 English technical terms you want to internalize]
```

### Why This Structure Works
- **One-Sentence Summary** trains compression — the hardest English skill
- **Key Concept Explained** trains the "explain to someone" muscle in English
- **Connection to My Work** makes it immediately useful, not academic
- **New Vocabulary** builds your technical English lexicon over time

## Directory Structure

```
ai-architect-journal/
├── README.md
├── CLAUDE.md                    # Claude Code instructions
├── templates/
│   ├── daily-entry.md           # Daily template
│   └── weekly-review.md         # Friday reflection template
├── entries/
│   └── 2026/
│       ├── 04-april/
│       │   ├── 2026-04-21-mon.md
│       │   ├── 2026-04-22-tue.md
│       │   └── ...
│       └── 05-may/
├── vocabulary/
│   └── master-list.md           # Running vocabulary list
└── reading-queue/
    └── queue.md                 # Articles to read next
```

## Recommended Sources

### Tier 1 — Weekly Must-Reads
- [Anthropic Research Blog](https://www.anthropic.com/research)
- [Google DeepMind Blog](https://deepmind.google/discover/blog/)
- [OpenAI Blog](https://openai.com/blog)
- [Hugging Face Blog](https://huggingface.co/blog)

### Tier 2 — Platform & Architecture
- [ServiceNow Developer Blog](https://developer.servicenow.com/blog.do)
- [ServiceNow Community — AI/ML](https://www.servicenow.com/community/ai-intelligence-articles/ta-p/2949486)
- [AWS Machine Learning Blog](https://aws.amazon.com/blogs/machine-learning/)
- [Google Cloud AI Blog](https://cloud.google.com/blog/products/ai-machine-learning)

### Tier 3 — Deep Dives
- [Distill.pub](https://distill.pub/) (interactive ML explainers)
- [Lilian Weng's Blog](https://lilianweng.github.io/) (comprehensive ML overviews)
- [The Gradient](https://thegradient.pub/)
- [arXiv — cs.AI](https://arxiv.org/list/cs.AI/recent) (scan titles, read selectively)

## Getting Started

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/ai-architect-journal.git
cd ai-architect-journal

# Create today's entry
cp templates/daily-entry.md entries/2026/04-april/$(date +%Y-%m-%d)-$(date +%a | tr '[:upper:]' '[:lower:]').md

# Write for 15 minutes, then commit
git add .
git commit -m "$(date +%Y-%m-%d): [topic]"
git push
```

## Weekly Review (Every Friday)

On Fridays, replace the daily entry with a weekly review (`templates/weekly-review.md`):
- What concepts stuck?
- What English patterns am I repeating? (overused words, awkward structures)
- What do I want to go deeper on next week?

## Progress Tracking

The git commit history IS the progress tracker. One commit per day = one green square on GitHub. The streak is the goal.
