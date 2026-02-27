# 🧠 Neural Lens (AI_BTS) — How AI Thinks
Ever wonder what actually happens when you type a message to an AI? This project shows you — step by step, in plain English and full technical detail.
## What is this?
**Neural Lens** is an interactive visual explainer that walks you through the 9 stages an AI model goes through every single time you send it a message — from the moment you hit send to the word it picks next.

It works for two kinds of people:

- 📖 **Story Mode** — No jargon. Real-world analogies. Anyone can understand it.
- ⚙️ **Deep Dive** — Full math derivations, attention matrices, step-by-step calculations. Built for engineers and the technically curious.

Type any message, hit **Analyze**, and watch your words travel through the entire AI pipeline in real time.

## What you'll see

| Stage | What happens |
|-------|-------------|
| 1 | **Tokenization** — Your message gets split into tokens using BPE |
| 2 | **Embeddings** — Each token becomes a 4096-dimensional vector |
| 3 | **Self-Attention** — The model figures out which words relate to each other |
| 4 | **96 Transformer Layers** — Deep processing, layer by layer |
| 5 | **KV Cache** — How the model remembers context efficiently |
| 6 | **Token Prediction** — Probability voting across 100,000 candidates |
| 7 | **Context Window** — What's actually inside every request |
| 8 | **Cost Calculator** — Real token costs across 5 different models |
| 9 | **Output Generation** — Word-by-word streaming with per-token cost |

## Key insights people always find surprising

- 🔥 Your message is **the cheapest part** of every API call — the system prompt is the real cost
- 🧠 AI has **zero memory** between conversations — it re-reads a full transcript every single time
- 🎲 The same question gets different answers because AI **samples from a probability distribution**, not a lookup table
- 💸 At 10,000 calls/day, a "tiny" system prompt overhead adds up to **$200+/month**

## Tech Stack

| Layer | Details |
|-------|---------|
| **Frontend** | Vanilla HTML, CSS, JavaScript — zero frameworks |
| **Fonts** | Syne, Nunito, JetBrains Mono via Google Fonts |
| **Animations** | Pure CSS keyframes + async JS pipeline |
| **Hosting** | GitHub Pages |
| **API** | None — fully static, runs entirely in the browser |

No build step. No npm install. No backend. Just one HTML file.

## Run it locally

No setup needed. Just:

1. Download `index.html`
2. Open it in any browser

That's it.

## Built by

**[@guru0203](https://github.com/guru0203)**

Built to make AI less of a black box — for everyone, not just engineers.

*If this helped you understand AI better, feel free to ⭐ the repo.*
