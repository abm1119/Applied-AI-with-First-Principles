# Deep Daily Curriculum Checklists
**Curriculum only.** Full guided checklists with explanations.

Use this file during the 6:00–8:30 PM block.

---

# PHASE 1 — Foundations (Days 1–14)

## Day 1 — What AI Engineering Is + Environment Setup
**Goal:** Understand the field clearly and have a clean working environment.

### Checklist
- [ ] Read or watch one solid explanation of “AI Engineering vs ML Research vs Data Science” (30–40 min)
- [ ] Write your own 5–7 sentence definition of AI Engineering in a notes file
- [ ] Install `uv` (or confirm it works)
- [ ] Create a new project folder: `ai-lab`
- [ ] Initialize with `uv init` + create virtual environment
- [ ] Create basic folder structure: `src/`, `notebooks/`, `notes/`, `experiments/`
- [ ] Write a clean README.md explaining what this lab is for
- [ ] Make first git commit and push to GitHub
- [ ] Write tomorrow’s one-sentence goal

### Why this matters
Most people jump into tools without knowing what problem AI Engineering actually solves. You need a clear mental model first. A clean environment removes friction for the next 99 days.

### Deep Guidance
Focus on the difference between:
- Training models (research)
- Using models to build reliable systems (engineering)

Your job for the next 100 days is the second one.

### Definition of Done
You can open the `ai-lab` repo on GitHub and explain in plain language what AI Engineering is.

---

## Day 2 — Pydantic v2 Deep Dive
**Goal:** Make Pydantic your default way to handle data.

### Checklist
- [ ] Read official Pydantic v2 overview (models, validation, settings)
- [ ] Create 3 real models:
  - `ChatMessage`
  - `LLMConfig`
  - `AppSettings` (using pydantic-settings)
- [ ] Add field validators to at least one model
- [ ] Write a small script that loads settings from `.env`
- [ ] Test what happens when invalid data is passed
- [ ] Commit the code with a clear message
- [ ] Write 3 bullet notes on why Pydantic beats raw dicts

### Why this matters
Almost every serious AI application uses structured data. Pydantic is the standard. Mastering it early saves hundreds of hours later.

### Deep Guidance
Pay special attention to:
- `model_validate` vs `model_dump`
- How settings can load from environment variables
- Custom validators

### Definition of Done
You can create a new Pydantic model in under 3 minutes and use it to validate incoming data.

---

## Day 3 — FastAPI Fundamentals for AI
**Goal:** Build your first AI-ready API endpoint.

### Checklist
- [ ] Create a FastAPI app inside `ai-lab`
- [ ] Define request and response models with Pydantic
- [ ] Create a `/health` endpoint
- [ ] Create a `/chat` endpoint that accepts a message and returns a dummy reply
- [ ] Test both endpoints with curl or the automatic docs
- [ ] Add basic error handling
- [ ] Commit and push
- [ ] Write notes: “Why FastAPI is a good fit for AI backends”

### Why this matters
You need a way to expose your AI logic. FastAPI is currently the best balance of speed, type safety, and developer experience.

### Deep Guidance
Use the automatic `/docs` page heavily today. Understand how Pydantic models become OpenAPI schemas.

### Definition of Done
You can start the server and successfully call `/chat` from another terminal.

---

## Day 4 — Streaming Responses
**Goal:** Make the API stream tokens like real chat products.

### Checklist
- [ ] Research how FastAPI streaming works (StreamingResponse)
- [ ] Modify `/chat` to stream a fake response token by token
- [ ] Test streaming with curl (`-N` flag) or a simple client
- [ ] Add a small delay between tokens so you can see it working
- [ ] Handle client disconnection cleanly if possible
- [ ] Commit the streaming version
- [ ] Write notes on why streaming matters for user experience

### Why this matters
Users hate waiting for the full response. Streaming is table stakes for any serious chat interface.

### Deep Guidance
Focus on understanding the generator pattern in Python and how FastAPI consumes it.

### Definition of Done
You can see tokens appearing one by one in the terminal.

---

## Day 5 — Configuration, Secrets & Docker Basics
**Goal:** Make the project production-aware.

### Checklist
- [ ] Move all secrets and config into `.env` + pydantic-settings
- [ ] Make sure `.env` is in `.gitignore`
- [ ] Write a simple Dockerfile for the FastAPI app
- [ ] Build the Docker image
- [ ] Run the container and test the endpoints
- [ ] Write a short note: “What I still don’t understand about Docker”
- [ ] Commit everything (except secrets)

### Why this matters
You will eventually deploy. Learning the basics of config and containers early prevents painful rewrites later.

### Deep Guidance
Do not try to learn all of Docker today. Just enough to containerize this one app.

### Definition of Done
You can run `docker build` and `docker run` and hit the API successfully.

---

## Day 6 — Review & Hardening
**Goal:** Make the foundation solid before moving on.

### Checklist
- [ ] Re-read all notes from Days 1–5
- [ ] Fix any messy code or unclear names
- [ ] Improve the README so a stranger can run the project
- [ ] Add a simple Makefile or just clear commands in the README
- [ ] Write a “Phase 1 so far” summary (10–15 lines)
- [ ] Identify the single weakest area
- [ ] Plan the weekend project clearly on paper

### Why this matters
Most people never stop to consolidate. This day turns scattered learning into durable skill.

### Definition of Done
The repo is clean enough that you would not be embarrassed to show it to another engineer.

---

## Day 7 — Weekend Project 1: Minimal LLM Chat API
**Goal:** Ship the first public artifact.

### Checklist
- [ ] Decide the exact scope (keep it small)
- [ ] Implement the core features
- [ ] Write a proper README with setup instructions
- [ ] Add at least one screenshot or simple demo
- [ ] Push to public GitHub
- [ ] Write a short LinkedIn post about what you built and what you learned
- [ ] Update `05-PROGRESS.md`

### Why this matters
Shipping is a skill. The first public repo is the hardest. After this it gets easier.

### Definition of Done
Anyone can find the repo, read the README, and understand what it does.

---

## Day 8 — LLM API Fundamentals
**Goal:** Make your first real LLM calls cleanly.

### Checklist
- [ ] Set up API keys safely (Grok / OpenAI / Anthropic — pick one main + one backup)
- [ ] Write a clean client wrapper function
- [ ] Make a successful non-streaming call
- [ ] Make a successful streaming call
- [ ] Log model name, tokens used, and latency
- [ ] Experiment with temperature and max_tokens
- [ ] Write notes on the differences you observed

### Why this matters
Raw API calls are the foundation of everything else. A clean client wrapper will be reused for months.

### Deep Guidance
Do not use a heavy framework yet. Stay close to the metal so you understand what is happening.

### Definition of Done
You have a reusable function that can call an LLM and return both the text and usage metadata.

---

## Day 9 — Structured Output
**Goal:** Force the LLM to return reliable, typed data.

### Checklist
- [ ] Learn the current recommended way to get structured output from your chosen provider
- [ ] Define a Pydantic model for the expected response
- [ ] Make the LLM return data that validates against the model
- [ ] Handle the case when validation fails (retry or repair)
- [ ] Build a small “structured note extractor” example
- [ ] Commit the code
- [ ] Write notes: “Why structured output changes everything”

### Why this matters
Free-form text is hard to build systems on. Structured output is how you make LLMs useful in real applications.

### Definition of Done
You can reliably get a Pydantic object back from the LLM.

---

## Day 10 — Tool / Function Calling
**Goal:** Let the LLM use tools.

### Checklist
- [ ] Understand how tool calling works with your provider
- [ ] Define one simple tool (e.g. calculator or get_current_time)
- [ ] Make the LLM decide when to call the tool
- [ ] Execute the tool and send the result back
- [ ] Complete the full loop
- [ ] Test both “needs tool” and “does not need tool” cases
- [ ] Commit and write short notes

### Why this matters
Tool calling is the bridge between language models and real action. This is the core of agents.

### Definition of Done
You have a working loop where the model can call a tool and use the result.

---

## Day 11 — Reliability Layer
**Goal:** Make the system robust.

### Checklist
- [ ] Add retries with exponential backoff
- [ ] Add timeout handling
- [ ] Add basic rate-limit awareness
- [ ] Create a simple cost tracker (input tokens + output tokens)
- [ ] Log every request cleanly
- [ ] Test failure cases deliberately
- [ ] Write notes on the failure modes you observed

### Why this matters
Real systems fail. The difference between a demo and a product is how you handle failure.

### Definition of Done
Your client can survive temporary API errors without crashing.

---

## Day 12 — Conversation Memory
**Goal:** Give the chat memory.

### Checklist
- [ ] Implement simple buffer memory (last N messages)
- [ ] Implement a basic summary memory approach
- [ ] Compare the two qualitatively
- [ ] Decide which one you prefer for now and why
- [ ] Integrate memory into your chat endpoint
- [ ] Test a multi-turn conversation
- [ ] Commit and document the decision

### Why this matters
Without memory, every conversation starts from zero. Even simple memory dramatically improves usefulness.

### Definition of Done
You can have a 5+ turn conversation that remembers earlier context.

---

## Day 13 — Full Phase 1 Review
**Goal:** Consolidate everything before the second weekend project.

### Checklist
- [ ] Re-read all notes from Days 1–12
- [ ] Run every major piece of code again
- [ ] Fix any broken or messy parts
- [ ] Update the main README of `ai-lab`
- [ ] Write a “Phase 1 Complete” summary (what you can now do)
- [ ] List the top 3 things that still feel fuzzy
- [ ] Plan the exact scope of Weekend Project 2

### Definition of Done
You can explain the entire stack you have built so far without looking at notes.

---

## Day 14 — Weekend Project 2: Structured Chat with Tools
**Goal:** Ship a more complete system.

### Checklist
- [ ] Combine structured output + tool calling + memory
- [ ] Keep scope tight
- [ ] Clean README + demo
- [ ] Public GitHub repo
- [ ] LinkedIn post explaining the architecture
- [ ] Update progress tracker

### Definition of Done
A working public project that demonstrates the core skills from Phase 1.

---

# PHASE 2 — Core LLM Engineering (Days 15–35)

### Daily Structure for this Phase
Every learning block follows this pattern:

1. Review previous day (10 min)
2. Learn the new concept (50–60 min)
3. Hands-on implementation (50–60 min)
4. Notes + content idea capture (10–15 min)
5. Tomorrow’s goal (5 min)

### Key Outcomes Required by Day 35
- [ ] Reliable structured output pipeline you trust
- [ ] Clean tool-calling loop
- [ ] At least two different memory strategies tested
- [ ] Cost and latency tracking in place
- [ ] Two additional public projects shipped
- [ ] Personal library of prompt patterns started

### Weekly Focus Suggestions
- Week 3: Advanced prompting + output repair loops
- Week 4: Component design (reusable client, memory, tools)
- Week 5: Evaluation of LLM outputs + hardening

---

# PHASE 3 — RAG Systems (Days 36–55)

### Daily Structure
Same as Phase 2, but every concept must end with a measurable retrieval experiment.

### Required Outcomes by Day 55
- [ ] Working embedding pipeline
- [ ] At least two chunking strategies compared
- [ ] Vector store integrated (Chroma first)
- [ ] Basic RAG evaluation running
- [ ] One complete RAG application shipped
- [ ] Second RAG project shipped

---

# PHASE 4 — Agents (Days 56–70)

### Required Outcomes by Day 70
- [ ] Single agent with multiple tools
- [ ] One planning pattern implemented (ReAct or Plan-Execute)
- [ ] Basic guardrails
- [ ] Two agent demos shipped

---

# PHASE 5 — Shipping & Observability (Days 71–85)

### Required Outcomes by Day 85
- [ ] One system actually deployed
- [ ] Logging and basic tracing added
- [ ] Evaluation loop running on real data
- [ ] Cost and latency notes written

---

# PHASE 6 — Advanced + Polish (Days 86–100)

### Required Outcomes by Day 100
- [ ] One larger personal project completed
- [ ] All previous repos cleaned and documented
- [ ] Final written reflection
- [ ] Next 100-day plan drafted

---

**How to use this file**
- Days 1–14: Follow the daily checklists exactly.
- Days 15+: Use the phase outcomes + daily structure.
- Always end the block by writing tomorrow’s one-sentence goal.
