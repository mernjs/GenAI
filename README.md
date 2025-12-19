# Python + GenAI

**Learn Generative AI by building real systems — step by step, in Python.**

This repository is a **hands-on, production-oriented learning path** for modern Generative AI.
It takes you from **first LLM calls** to **full-scale AI products** involving RAG, agents, vision, diffusion models, and deployment.

Everything here is designed to be:

* Practical
* Incremental
* Production-minded
* Easy to reason about and extend

No black boxes.
You **build every layer yourself**.

---

## What this repository is about

This is **not a theory repo**.
This is a **build-first GenAI repository**.

You will:

* Write real Python code
* Debug real problems (context limits, hallucinations, latency)
* Build reusable components
* Understand *why* systems break — and how to fix them
* Move from prompts → systems → products

Each folder represents **one concrete project**, focused on a **single GenAI concept**, implemented cleanly and explained clearly.

---

## Learning philosophy

This repository follows four principles:

1. **Hands-on first**
   Every concept is learned by building something tangible.

2. **Progressive complexity**
   Each project builds directly on previous ones.

3. **Production realism**
   Topics like evaluation, guardrails, memory, orchestration, and deployment are first-class.

4. **System-level thinking**
   You learn how components fit together — not just how to call an API.

---

## What this repository includes

Projects are organized in a **strict learning order**, from fundamentals to advanced, real-world systems.

### Core Foundations

* What Generative AI really is
* How LLMs work internally
* Tokens, context windows, cost, latency
* Prompt structure and behavior control

### Prompting & Conversation

* Prompt engineering patterns
* System vs user vs assistant roles
* Conversation state management
* Short-term and long-term memory

### Embeddings & Search

* Vector embeddings from scratch
* Semantic similarity and ranking
* Chunking strategies
* Metadata-aware retrieval

### Retrieval-Augmented Generation (RAG)

* PDF and document Q&A
* Query rewriting
* Hybrid retrieval (keyword + vector)
* Re-ranking and long-context strategies
* Multi-source knowledge systems

### Agents & Tooling

* Tool calling and function execution
* Planner–executor agents
* Multi-agent collaboration
* Workflow orchestration
* Autonomous agents with guardrails

### Reliability, Safety & Evaluation

* Hallucination detection
* Confidence scoring
* Prompt and model regression testing
* Evaluation pipelines
* Error handling and fallbacks

### Production Systems

* API design
* Observability and monitoring
* Versioning and experiment tracking
* Security and access control
* Scalable architectures

### Advanced AI 

* LLM fine-tuning (SFT, LoRA, PEFT)
* Domain-specific models
* Computer Vision with YOLO
* Multimodal systems
* Diffusion and Stable Diffusion
* Full-stack AI products

---

## Project-based structure (what you actually build)

Each project folder contains:

* Clear goal
* Minimal but complete implementation
* Focused scope (one core idea)
* Code you can reuse in real systems

You don’t just *learn about*:

* RAG → you build multiple RAG systems
* Agents → you build planners, executors, and workflows
* Vision → you run YOLO and connect it to LLMs
* Diffusion → you generate, fine-tune, and edit images

---

## From beginner to advanced — without gaps

This repo is designed so that:

* Beginners can start from project 1
* Experienced engineers can jump to any phase
* No conceptual leaps are required
* Every advanced topic is grounded in earlier work

By the end, you will understand:

* How GenAI systems actually work
* How to design them cleanly
* How to debug and evaluate them
* How to ship them responsibly

---

## Who this is for

This repository is ideal for:

* Developers learning Generative AI seriously
* Backend or full-stack engineers adding AI features
* Engineers transitioning into GenAI roles
* Builders creating real AI-powered products
* Anyone who prefers **code over slides**

If you like learning by **building systems**, this repo is for you.

---

## How to use this repository

Recommended approach:

1. Start from Project 01 and move forward
2. Run every project locally
3. Modify and break things
4. Reuse components across projects
5. Treat this as a personal GenAI toolkit

You can also:

* Use it as a course
* Use it as a reference
* Use it as a portfolio foundation

---

## License

MIT — free to use, modify, and build on.