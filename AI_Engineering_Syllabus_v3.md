# AI Engineering Master Syllabus (v3 — Complete 100 Days Plan)

This syllabus represents the definitive 100-Day Master Curriculum in Applied AI Engineering. It bridges academic theory with practical application, integrating your daily study routines (weekday learning and research) and weekend building sprints with high-quality online textbooks, official documentation, whitepapers, and curated repositories.

---

## 📅 Daily Study Schedule Alignment
*   **Weekday AI Study Block (6:00 PM – 8:30 PM | 2.5 Hrs):** Applied engineering, architectural patterns, framework documentation, and coding labs.
*   **Weekday Research & Paper Block (11:30 PM – 2:00 AM | 2.5 Hrs):** Literature analysis, research drafting in LaTeX, baseline evaluations, and experiment tracking.
*   **Weekend Learn & Build Block (4:00 PM – 9:30 PM | 5.5 Hrs):** Large-scale coding, full-stack database and service integration, and open-source repository uploads.
*   **Weekend YouTube Content Block (11:00 AM – 4:00 PM | 5.0 Hrs):** Technical scriptwriting, software demonstrations, and screen-cast filming.

---

## 🗺️ Curriculum Phase Overview

```
Phase 1: Diffusion & Generative Media ────────────────────── Weeks 1-3  (Days 01-21)
Phase 2: LLM Core & Full-Stack AI Engineering ────────────── Weeks 4-8  (Days 22-56)
Phase 3: Agentic Systems & Multi-Agent Loops ─────────────── Weeks 9-11 (Days 57-77)
Phase 4: Evals, Guardrails, & Production Fine-Tuning ─────── Weeks 12-13 (Days 78-91)
Phase 5: Advanced Production Ops & Capstone Showcases ────── Week 14+   (Days 92-100)
```

---

## 🎨 Phase 1: Diffusion & Generative Media (Days 1–21)
*Focus: Mastering latent space architectures, conditional diffusion layers, advanced ComfyUI orchestration, and automated marketing campaigns.*

### Week 1 (Days 1–7): Diffusion Foundations & UI Tools
*   **Day 1: Foundations of Latent Diffusion Models (LDMs)**
    *   *Topics:* Core diffusion process (forward and reverse), noise-to-image math, and UNet architectures.
    *   *Reading:* Simon Prince's *Understanding Deep Learning*, Chapter 18 (Diffusion Models).
    *   *Assignment:* Set up a mathematical noise grid showing diffusion steps.
*   **Day 2: Understanding CLIP Text Encoders & Noise Schedules**
    *   *Topics:* Embedding text prompts, conditional embeddings, and denoising schedulers (DDIM, Euler, DPM++).
    *   *Reading:* Stanford's *Speech and Language Processing*, Chapter 10 (Transformers) for sequence representations.
    *   *Assignment:* Track and plot the mathematical progression of noise reduction across 20 steps.
*   **Day 3: Prototyping with Fooocus Lab**
    *   *Topics:* Prompt-based optimization, style templates, in-painting, and mid-journey styled parameters.
    *   *Guide:* *Fooocus Lab Github Repository* for CLI setup and model installations.
    *   *Assignment:* Generate 5 distinct artistic style generations using Fooocus CLI parameters.
*   **Day 4: Deep Dive into ComfyUI Node Architectures**
    *   *Topics:* Computational graphs, input/output structures (LATENT vs IMAGE vs MODEL), and installing custom nodes.
    *   *Docs:* *ComfyUI GitHub and Wiki Documentation*.
    *   *Assignment:* Install ComfyUI-Manager and construct your first txt2img node flowchart.
*   **Day 5: Text-to-Image (TXT2IMG) Workflows**
    *   *Topics:* Loaders, Prompters, KSamplers, and VAE Decoders.
    *   *Resource:* *ComfyUI Starter Manual & Workflows*.
    *   *Assignment:* Build and export a standard SD1.5/SDXL txt2img ComfyUI workflow JSON.
*   **Day 6: Image-to-Image (IMG2IMG) Workflows**
    *   *Topics:* VAE Encoders, latent denoising parameters, and image processing.
    *   *Resource:* *ComfyUI Tutorials*.
    *   *Assignment:* Construct an IMG2IMG workflow that takes a hand-drawn sketch and transforms it into high-fidelity concept art.
*   **Day 7: Scaling Latents & Mastering Negative Prompts**
    *   *Topics:* CFG Scale mechanics, Latent Upscaling (Hi-Res Fix), and negative embedding embeddings.
    *   *Resource:* *Aifoundations.school - Diffusion Module*.
    *   *Assignment:* Compare visual outputs across varying CFG settings (3, 7, 12, 20) and document structural changes.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Select target title and research questions. Set up Zotero library and Better BibTeX formatting. Collect first 10 papers on Small Language Model (SLM) applications in educational settings.
*   **🛠️ Weekend Lab 1 (4:00 PM - 9:30 PM):** Assemble a modular, group-categorized ComfyUI starter template. Export as JSON and upload to a public GitHub repo.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"ComfyUI Zero-to-Hero: Complete Installation & Visual Pipeline Setup."*

### Week 2 (Days 8–14): Advanced ComfyUI Conditioning & Models
*   **Day 8: Architecture Comparison: SDXL vs. Flux.1**
    *   *Topics:* DiT (Diffusion Transformer) pipelines, Flux Dev vs. Flux Schnell, Flux Kontext, and Flux Redux.
    *   *Resource:* *Hugging Face Spaces for Flux.1 model explorations*.
    *   *Assignment:* Benchmark memory allocation and generation times comparing SDXL vs. Flux Schnell.
*   **Day 9: ControlNet Engineering**
    *   *Topics:* Canny, Depth, OpenPose, and Scribble conditioning layers.
    *   *Guide:* *Anthropic Tool Use (Function Calling) Cookbook* (concept of structure and parameters).
    *   *Assignment:* Build a ComfyUI pipeline that extracts pose coordinates from an input image and maps them to a new character.
*   **Day 10: IP-Adapters (Image Prompt Adapters)**
    *   *Topics:* Image-based style reference injections, face-similarity mapping, and weights.
    *   *Resource:* *Advanced ComfyUI Playbook*.
    *   *Assignment:* Feed a brand logo into an IP-Adapter and generate a themed commercial wallpaper.
*   **Day 11: Advanced Inpainting & Outpainting Workflows**
    *   *Topics:* Masking models, prompt-guided object replacement, and border extensions.
    *   *Resource:* *Fooocus Lab Inpaint Documentation*.
    *   *Assignment:* Mask out a target product from a photo and replace its background cleanly while maintaining object shadows.
*   **Day 12: Custom Face Swapping with ReActor & InsightFace**
    *   *Topics:* Face restore models, face analysis, and multi-character masking.
    *   *Resource:* *ComfyUI Custom Node Directories*.
    *   *Assignment:* Build a face-swapping pipeline that restores facial details using CodeFormer or GFPGAN.
*   **Day 13: Image-to-Text with Qwen2-VL**
    *   *Topics:* Visual-Language Models (VLMs), captioning datasets, and structured scene descriptions.
    *   *Resource:* *Google Gemini Developer Cookbook (Multimodal section)*.
    *   *Assignment:* Feed 10 generated images to Qwen2-VL to auto-generate highly detailed descriptive alt-text metadata.
*   **Day 14: Complex Flow Routing & Group Orchestration**
    *   *Topics:* Switch nodes, custom bypass rules, annotation layers, and group layouts.
    *   *Resource:* *ComfyUI-Manager advanced node guides*.
    *   *Assignment:* Refactor your previous workflows into a single, clean multi-path master workspace.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Literature search on SLM fine-tuning and token-efficiency patterns. Read and catalog 15 papers in Zotero.
*   **🛠️ Weekend Lab 2 (4:00 PM - 9:30 PM):** Build an image-guided remastering desktop script using a ComfyUI headless API python wrapper.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"The Flux Revolution: High-Fidelity Image Generation in ComfyUI."*

### Week 3 (Days 15–21): Custom Models, Video Generation, & Campaigns
*   **Day 15: LoRA (Low-Rank Adaptation) Visual Theory**
    *   *Topics:* Weight matrices, ranks (dimension scaling), and visual style dataset curation.
    *   *Paper:* *Hu et al., "LoRA: Low-Rank Adaptation of Large Language Models"* (adaptation of ranks).
    *   *Assignment:* Prepare 20 high-resolution images of a unified object or style, crop, and write text captions.
*   **Day 16: Configuring Custom LoRA Training Scripts**
    *   *Topics:* Learning rates, epochs, optimizer settings (AdamW, Adafactor), and checkpointing.
    *   *Resource:* *Kohya_ss or Axolotl Fine-Tuning Setup guides*.
    *   *Assignment:* Configure and dry-run a local trainer YAML config file.
*   **Day 17: Testing & Weight-Tuning Custom LoRAs**
    *   *Topics:* Merging models, dynamic prompt triggers, and weight evaluations.
    *   *Resource:* *Hugging Face PEFT Library guides*.
    *   *Assignment:* Generate grid comparisons showing outputs of your custom LoRA evaluated from weights 0.1 to 1.2.
*   **Day 18: AI Video Generation Foundations**
    *   *Topics:* Temporal consistency, Wan Animate, SkyReels, and Infinite-Talk.
    *   *Resource:* *Hugging Face Spaces - Wan-2.1 and SkyReels*.
    *   *Assignment:* Render a 4-second consistent video clip from a text description using a local space endpoint.
*   **Day 19: Audio-Reactive Visual Generations**
    *   *Topics:* Audio spectrum extraction, frequency mapping to latent parameters, and keyframing.
    *   *Resource:* *ComfyUI-Audio nodes manual*.
    *   *Assignment:* Build a video pipeline where camera motion reacts dynamically to the bass-line of an audio track.
*   **Day 20: Narrative Ads via TTS Engine Injections**
    *   *Topics:* Kokoro TTS, ElevenLabs APIs, sub-title overlays, and automated timeline generation.
    *   *Resource:* *Dave Ebbelaar's Voice Cloning and Video Pipeline guides*.
    *   *Assignment:* Generate a voiceover track, generate matching video clips, and stitch them programmatically using MoviePy.
*   **Day 21: Automating Complete Multi-Media Campaigns**
    *   *Topics:* Batch generation, folder tracking, and bulk asset exports.
    *   *Resource:* *Patterns of Application Development Using AI - Automation chapters*.
    *   *Assignment:* Create a Python script that takes a single campaign slogan, generates 10 unique product background images, and packages them into a compressed folder.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Formalize the experimental educational tasks. Outline metrics for evaluation. Write the draft Introduction and Problem Statement sections in Overleaf.
*   **🛠️ Weekend Lab 3 (4:00 PM - 9:30 PM):** Launch an automated marketing content generator that consumes an API feed, spins up a headless ComfyUI container, and renders structured ads.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"How to Train Your Own ComfyUI LoRA in Under 30 Minutes."*

---

## 🛠️ Phase 2: LLM Core & Full-Stack AI Engineering (Days 22–56)
*Focus: Executing spec-driven development, building asynchronous API backends, designing persistent storage ERDs, and configuring robust RAG indexing.*

### Week 4 (Days 22–28): Idea Validation & Spec-Driven Development
*   **Day 22: Applying the 5-Layer AI Validation Framework**
    *   *Topics:* Problem reality, AI necessity, data feasibility, evals, and distribution analysis.
    *   *Reading:* *How to Validate an AI Idea*, Sections 1 & 2.
    *   *Assignment:* Perform a formal 5-layer audit on your proposed Educational SLM Mentor application.
*   **Day 23: Writing the One-Page Idea Card**
    *   *Topics:* Problem statements, target users, alternative solutions, and proposed success metrics.
    *   *Reading:* *How to Validate an AI Idea*, Section 3 & 6.
    *   *Assignment:* Draft and submit your educational AI agent Idea Card in markdown.
*   **Day 24: Conducting the "Mom Test" User Interviews**
    *   *Topics:* Neutral questioning, extracting behavioral histories, and avoiding positive bias.
    *   *Reading:* *How to Validate an AI Idea*, Day 3-5 Conversations.
    *   *Assignment:* Script 5 unbiased interview questions and draft mock answers mimicking a high-school student.
*   **Day 25: Crafting the Initial Golden Dataset**
    *   *Topics:* JSONL formats, input-output pairing, mapping common vs. edge cases.
    *   *Reading:* *How to Create a Golden Dataset*, Sections 1 & 3.
    *   *Assignment:* Manually compile a 15-example Golden Dataset representing high-school algebra questions and perfect pedagogical explanations.
*   **Day 26: Spec-Driven Development (SDD): Drafting the PRD**
    *   *Topics:* Product Requirement Documents, architecture scopes, and API endpoints definitions.
    *   *Resource:* *Mattpocock/skills Repository - Interface patterns*.
    *   *Assignment:* Write a detailed PRD defining the data schemas and latency budgets for your educational API.
*   **Day 27: Test-Driven Development (TDD) for Prompt Pipelines**
    *   *Topics:* Assertions, deterministic tests, and prompt test frameworks.
    *   *Resource:* *Mattpocock/skills - Testing configurations*.
    *   *Assignment:* Write 3 unit tests using PyTest to validate that an LLM response matches expected JSON formats.
*   **Day 28: Fast Mock Interfaces in Streamlit**
    *   *Topics:* Streamlit widgets, state sessions, and mock API loops.
    *   *Resource:* *Dave Ebbelaar's Streamlit Guides*.
    *   *Assignment:* Code a clean multi-turn chatbot UI that reads from mock static responses.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Set up local baseline environment with Llama-3-8B-Instruct. Build basic baseline evaluation script. Create a localized dataset directory.
*   **🛠️ Weekend Lab 4 (4:00 PM - 9:30 PM):** Create a automated schema validator script in Python that consumes raw texts, passes them to a structural model, and asserts output integrity against a Pydantic class.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Why Your AI Startup Idea Will Fail (And How to Validate It First)."*

### Week 5 (Days 29–35): Backend APIs & Asynchronous Servers
*   **Day 29: FastAPI Deep Dive: Schemas & Responses**
    *   *Topics:* FastAPI initialization, Pydantic BaseModels, type hinting, and response routing.
    *   *Docs:* *FastAPI Official Documentation*.
    *   *Assignment:* Build a FastAPI server that validates incoming student requests and returns structured mock results.
*   **Day 30: Asynchronous Coding (`async/await`)**
    *   *Topics:* Event loops, thread workers, non-blocking network calls, and concurrency.
    *   *Reading:* *Designing Data-Intensive Applications*, Chapter 5 (Asynchronous operations).
    *   *Assignment:* Write a script making 20 concurrent async mock LLM calls and measure elapsed time.
*   **Day 31: Entity-Relationship Diagram (ERD) Modeling**
    *   *Topics:* User accounts, dynamic conversation sessions, messages schema, and foreign keys.
    *   *Reading:* *Designing Data-Intensive Applications*, Chapter 2 (Data Models).
    *   *Assignment:* Sketch an ERD diagram mapping a multi-user, multi-chat architecture with timestamps.
*   **Day 32: Persistent Databases with SQL & SQLAlchemy**
    *   *Topics:* SQL queries, SQLite configurations, ORM sessions, and migrations.
    *   *Reading:* *Patterns of Application Development Using AI - Database persistent layers*.
    *   *Assignment:* Implement an SQLAlchemy script that saves conversation tables and retrieves a historical user chat log.
*   **Day 33: Streaming Responses (`StreamingResponse`)**
    *   *Topics:* SSE (Server-Sent Events), generator loops, and chunk parsing.
    *   *Docs:* *FastAPI StreamingResponse manual*.
    *   *Assignment:* Code a FastAPI endpoint that streams output text from an OpenAI call character-by-character.
*   **Day 34: Authentication & Rate Limiting Middleware**
    *   *Topics:* JWT tokens, secure headers, Redis caches, and throttling.
    *   *Resource:* *Chai aur Code's Backend series*.
    *   *Assignment:* Add a middleware layer that rejects requests exceeding 5 calls per minute from a single IP.
*   **Day 35: Backend Containerization with Docker**
    *   *Topics:* Dockerfiles, multi-stage builds, port mappings, and compose files.
    *   *Resource:* *Full Stack Deep Learning (FSDL) - Deployment guides*.
    *   *Assignment:* Package your FastAPI application into a Docker container and run it on a local port.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Test and log response times on your local model. Compare latency benchmarks when using FP16 vs. INT4 quantization.
*   **🛠️ Weekend Lab 5 (4:00 PM - 9:30 PM):** Launch a fully Dockerized, persistent Chat API that accepts user inputs, logs them in SQLite, and streams contextual answers back.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Building Asynchronous AI Backends with FastAPI & SQLite."*

### Week 6 (Days 36–42): Tool Calling & Model Context Protocol (MCP)
*   **Day 36: Understanding Tool/Function Calling**
    *   *Topics:* JSON schema tool parameters, model reasoning states, and extraction pipelines.
    *   *Guide:* *OpenAI Tool Calling Reference Guide*.
    *   *Assignment:* Formulate tool calling schemas for a "calculator" and a "web searcher".
*   **Day 37: Resilient Tool Error Handling & Fallbacks**
    *   *Topics:* Exception catches, error logging, and feeding traceback contexts back to models.
    *   *Resource:* *Anthropic Tool Use (Function Calling) Cookbook*.
    *   *Assignment:* Write a script that catches tool schema validation errors, prompts the LLM to correct itself, and re-runs the tool.
*   **Day 38: Model Context Protocol (MCP) Architecture**
    *   *Topics:* Host-Client relationships, transport protocols (Stdio vs SSE), and schema specifications.
    *   *Docs:* *Model Context Protocol (MCP) Documentation*.
    *   *Assignment:* Create a detailed block diagram explaining how MCP connects localized data silos to Claude Desktop.
*   **Day 39: Coding a Custom Python MCP Client**
    *   *Topics:* Client sessions, registering capabilities, and executing remote tools.
    *   *Docs:* *MCP Python SDK Manual*.
    *   *Assignment:* Code a lightweight Python script that acts as an MCP client and initiates tool sessions.
*   **Day 40: Building custom MCP Servers**
    *   *Topics:* Serving resources, exposing directories, and mapping filesystem APIs.
    *   *Resource:* *Awesome-MCP repositories (punkpeye)*.
    *   *Assignment:* Write a custom MCP server that serves an indexed local mathematical text book as a readable resource.
*   **Day 41: Advanced MCP Applications & Tool Nesting**
    *   *Topics:* Multi-schema structures, dynamic schema registration, and security constraints.
    *   *Resource:* *BuildWithHussain YouTube - MCP configurations*.
    *   *Assignment:* Implement an MCP tool that calls another nested tool, returning aggregated results.
*   **Day 42: Dynamic Security Sandbox Gateways**
    *   *Topics:* Sandboxed execution (Docker/Wasm), standard IO isolations, and authorization tokens.
    *   *Resource:* *Full Stack Deep Learning (FSDL) - Security modules*.
    *   *Assignment:* Build a tool-execution gateway that isolates file-writing scripts in a dynamic sandbox.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Test the local SLM's capability to format tool calling queries correctly. Record success and failure ratios on 50 runs.
*   **🛠️ Weekend Lab 6 (4:00 PM - 9:30 PM):** Create a custom MCP server that queries your SQLite database, wraps it in secure schemas, and connects to Claude Desktop for analytical reporting.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Anthropic's Model Context Protocol (MCP): The Future of AI Tooling."*

### Week 7 (Days 43–49): Advanced RAG & Retrieval Datasets
*   **Day 43: Mapping the Full Retrieval Pipeline**
    *   *Topics:* Ingestion, parsing, chunking, embedding, indexing, querying, and ranking.
    *   *Reading:* *How to Make a RAG-Ready Dataset*, Sections 1 & 2.
    *   *Assignment:* Draw a pipeline flow chart highlighting the differences between dense vector indexing and lexical BM25 indexing.
*   **Day 44: Text Extraction & Normalizations**
    *   *Topics:* Parsing PDFs/Markdown, stripping page navigation structures, fixing broken encodings, and Unicode cleaning.
    *   *Reading:* *How to Make a RAG-Ready Dataset*, Section 3 (Step 2).
    *   *Assignment:* Write a python parser script using PyPDF and MarkItDown that cleans headers/footers from standard educational papers.
*   **Day 45: Strategic Document Chunking**
    *   *Topics:* Character splitting vs. Semantic paragraph boundaries, overlaps, and parent-child hierarchies.
    *   *Reading:* *How to Make a RAG-Ready Dataset*, Section 3 (Step 3).
    *   *Assignment:* Build a parser comparing standard recursive chunking with document structure-aware chunking on a math textbook.
*   **Day 46: Metadata Enrichment Pipelines**
    *   *Topics:* Attaching source IDs, generating summary tags, and building hypothetical questions.
    *   *Reading:* *How to Make a RAG-Ready Dataset*, Section 3 (Step 4).
    *   *Assignment:* Process a folder of curriculum guidelines, appending generated "focus categories" and "difficulty levels" to each chunk.
*   **Day 47: Embedding & Vector DB Indexing**
    *   *Topics:* Selecting embedding dimensions, cosine similarity math, setting up Chroma or Qdrant indices.
    *   *Resource:* *DataTalksClub LLM Zoomcamp repositories*.
    *   *Assignment:* Set up a local Chroma client, embed 100 chunks using a Hugging Face model, and search.
*   **Day 48: Hybrid Search & Reranking**
    *   *Topics:* Reciprocal Rank Fusion (RRF), BM25 lexical integrations, and Cohere Rerank APIs.
    *   *Resource:* *Cohere RAG Optimization Guide & LLM University*.
    *   *Assignment:* Implement a hybrid search function in Python that returns dense results filtered by BM25 relevance scores.
*   **Day 49: Metric Evaluations for Retrieval**
    *   *Topics:* Recall@k, Mean Reciprocal Rank (MRR), and NDCG metrics.
    *   *Reading:* *How to Make a RAG-Ready Dataset*, Section 3 (Step 7).
    *   *Assignment:* Set up 30 test questions with known golden chunks, query your vector index, and calculate your system's Recall@5 score.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Draft the Method and Experimental Setup sections of your paper. Incorporate latency graphs and hardware specs [57].
*   **🛠️ Weekend Lab 7 (4:00 PM - 9:30 PM):** Code an automated document indexing tool that extracts clean markdown sections, generates parent-child relations, embeds them, and uploads vectors.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Stop Scraping PDFs: The Correct Way to Build RAG-Ready Datasets."*

### Week 8 (Days 50–56): Memory & Context Engineering
*   **Day 50: Conversational State Management**
    *   *Topics:* Short-term session parameters vs. Persistent semantic memory buffers.
    *   *Reading:* *Patterns of Application Development Using AI - Memory chapters*.
    *   *Assignment:* Sketch a memory life-cycle flow mapping user queries to historical summaries.
*   **Day 51: Persistent Memory with Redis & Postgres**
    *   *Topics:* Redis hashes, TTL (Time-To-Live), and saving vector embeddings of user queries.
    *   *Resource:* *Dave Ebbelaar's Database Persistent guides*.
    *   *Assignment:* Implement a Python script that stores user chat logs in PostgreSQL and caches session IDs in Redis.
*   **Day 52: Dynamic Context Window Compressions**
    *   *Topics:* Context pruning, summary generation on older messages, and token limit alerts.
    *   *Resource:* *LLM-Bento memory guides*.
    *   *Assignment:* Write a chat buffer script that automatically summarizes messages when context exceeds 4,000 tokens.
*   **Day 53: Sliding Window Memory**
    *   *Topics:* Fixed message loops, memory decay factors, and maintaining system prompts.
    *   *Resource:* *Aman's AI state patterns*.
    *   *Assignment:* Code a custom conversational loop that preserves the last 5 messages while injecting historical summaries.
*   **Day 54: Prompt Caching Configurations**
    *   *Topics:* Claude prompt caching boundaries, block layouts, and optimizing system prompts.
    *   *Docs:* *Anthropic Developer Prompt Caching docs*.
    *   *Assignment:* Re-arrange a 10,000-token educational prompt to ensure the static textbook resource is fully cached.
*   **Day 55: Full System Ingestions & Integrations**
    *   *Topics:* Connecting APIs, vector stores, Redis memory, and database logs into a single loop.
    *   *Resource:* *Applied AI Cookbooks (techwithram)*.
    *   *Assignment:* Connect all modular pipelines you built in Phase 2 into a single working local controller.
*   **Day 56: MVP-1 Deployment & Local Testing**
    *   *Topics:* Sandbox deployments, monitoring error rates, and load testing.
    *   *Resource:* *FSDL Deployment best practices*.
    *   *Assignment:* Deploy your full MVP-1 locally and run a automated load test sending 50 parallel requests.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Review final draft sections of your research paper in Overleaf. Compile LaTeX structure, references file, and figures [57, 58].
*   **🛠️ Weekend Lab 8 (4:00 PM - 9:30 PM):** Launch an interactive Conversational Educational Mentor platform that loads contextual history via semantic memory lookups and leverages prompt caching.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"How to Build AI Systems with Long-Term Memory and Context Engines."*

---

## 🧠 Phase 3: Agentic Systems & Multi-Agent Loops (Days 57–77)
*Focus: Implementing autonomous ReAct patterns, supervisor routing structures, state-machine synchronization, and loop engineering.*

### Week 9 (Days 57–63): Foundation of Autonomous Agents
*   **Day 57: Paradigm Shift: Code vs. Loop Reasoning**
    *   *Topics:* Static sequential calls vs. Autonomous loop states, and the ReAct paradigm.
    *   *Paper:* *Yao et al., "ReAct: Synergizing Reasoning and Acting in Language Models"*.
    *   *Assignment:* Write a manual trace showing the difference in steps when a model answers a multi-hop query with vs. without ReAct.
*   **Day 58: Modeling Agent States**
    *   *Topics:* Structuring shared memory states, transaction logs, and action history queues.
    *   *Resource:* *Lilian Weng's "LLM-Powered Autonomous Agents"*.
    *   *Assignment:* Define a JSON schema representing the state variables of an agentic learning solver.
*   **Day 59: Coding pure Python State-Machine Agents**
    *   *Topics:* While-loops, state switch cases, tool schemas, and parsing text streams.
    *   *Resource:* *BuildWithHussain - Custom Agent Coding loops*.
    *   *Assignment:* Build an agent from scratch in pure Python using a standard `while` loop that resolves a math task by executing a local file utility.
*   **Day 60: Action Parsing & Exception Recoveries**
    *   *Topics:* Capturing malformed JSON, dealing with missing parameters, and prompt error feedback loops.
    *   *Resource:* *Anthropic Tool Use (Function Calling) Cookbook*.
    *   *Assignment:* Write an agent execution loop that catches Python exceptions and feeds them back to the LLM to auto-debug.
*   **Day 61: Introduction to Agentic Graph Frameworks (LangGraph)**
    *   *Topics:* Nodes, Edges, Stateful Graphs, and conditional routings.
    *   *Resource:* *LangGraph and LangChain cookbooks*.
    *   *Assignment:* Construct a simple 3-node graph: Node A (User Input) -> Node B (Analyzer) -> Node C (Result).
*   **Day 62: Defining Dynamic Agentic Skills**
    *   *Topics:* Dynamic skill registries, code-as-a-tool integrations, and runtime loading.
    *   *Resource:* *Mattpocock/skills modularity patterns*.
    *   *Assignment:* Code an agent system that can read new Python functions from a text folder and registers them as usable tools on the fly.
*   **Day 63: Hand-on Lab: Triaging Support Systems**
    *   *Topics:* Multi-route analysis, priority classifications, and auto-reply tools.
    *   *Resource:* *Dave Ebbelaar's Agentic Triage Tutorials*.
    *   *Assignment:* Build a support agent that reads emails and routes them to high, medium, or low priority paths.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Analyze search results and citations on error-recovery patterns in localized SLMs. Map out patterns.
*   **🛠️ Weekend Lab 9 (4:00 PM - 9:30 PM):** Create a personalized Learning-Mentor Agent that analyzes a student's profile, plans an optimized syllabus, and fetches textbook sections via RAG.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Code Your First Autonomous AI Agent in Python (No Frameworks!)."*

### Week 10 (Days 64–70): Multi-Agent Collaboration & Supervisor Networks
*   **Day 64: Multi-Agent Topology Frameworks**
    *   *Topics:* Orchestrated networks, peer networks, and centralized vs. decentralized communications.
    *   *Resource:* *Lilian Weng's Agentic blog posts*.
    *   *Assignment:* Sketch a coordination flow comparing a sequential multi-agent chain with a centralized network.
*   **Day 65: Designing Supervisor Networks**
    *   *Topics:* Task routers, supervisor state transitions, and sub-agent dispatching.
    *   *Resource:* *LangGraph Supervisor Node templates*.
    *   *Assignment:* Build a supervisor agent in Python that parses a homework assignment and delegates tasks to a researcher agent and a writer agent.
*   **Day 66: Managing Shared State Consistency**
    *   *Topics:* Thread locking, state merges, dynamic context updates, and conflict avoidance.
    *   *Reading:* *Systems Thinking: Managing Chaos and Complexity*, Chapter 8.
    *   *Assignment:* Implement a memory store that locks state changes when two agents attempt to update the same chat variable simultaneously.
*   **Day 67: Conflict Resolution Patterns**
    *   *Topics:* Critic networks, consensus voting, and programmatic validators.
    *   *Resource:* *Eugene Yan's Multi-Agent Evaluations*.
    *   *Assignment:* Create a two-agent debate system where Agent A writes code and Agent B reviews it, executing only when Agent B approves.
*   **Day 68: Async Communications via Message Queues**
    *   *Topics:* Celery tasks, Redis brokers, message packaging, and background worker threads.
    *   *Resource:* *Chai aur Code's Celery & Redis tutorials*.
    *   *Assignment:* Set up an async worker queue that routes heavy agent analysis tasks to background workers while keeping the FastAPI server responsive.
*   **Day 69: Human-In-The-Loop (HITL) Intercepts**
    *   *Topics:* Approval nodes, state pauses, wait conditions, and resume routes.
    *   *Resource:* *LangGraph Human-In-The-Loop guides*.
    *   *Assignment:* Build an agent that drafts automated emails but pauses for human review and input before executing.
*   **Day 70: Technical Documentation Multi-Agent Team**
    *   *Topics:* Code analysis, markdown generation, cross-referencing, and verification.
    *   *Resource:* *Full Stack Deep Learning (FSDL) - Automated QA*.
    *   *Assignment:* Build a two-agent system that ingests a Python script, writes documentation, and validates file exports.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Test multi-agent evaluation frameworks. Record error patterns and run comparisons.
*   **🛠️ Weekend Lab 10 (4:00 PM - 9:30 PM):** Build a complete Multi-Agent content production team with sequential state passing: Agent 1 (Researcher), Agent 2 (Scriptwriter), Agent 3 (Editor).
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Multi-Agent Systems: Building Collaborative AI Development Teams."*

### Week 11 (Days 71–77): Harness Engineering & Loop Engineering
*   **Day 71: Harness Engineering Foundations**
    *   *Topics:* Surrounding weak models with robust code, sanitizing inputs, and enforcing static validation checks.
    *   *Reading:* *Mattpocock/skills - Harness architectures*.
    *   *Assignment:* Write a wrapper around a 3B SLM tool caller that catches syntax omissions and repairs them with Python code.
*   **Day 72: Loop Engineering & Critique-Refine Cycles**
    *   *Topics:* Iterative improvement loops, score thresholds, self-reflection mechanisms.
    *   *Resource:* *Aman's AI Loop implementations*.
    *   *Assignment:* Code an agent that receives an essay draft, grades itself against a rubric, and rewrites the draft until it scores above 80%.
*   **Day 73: Compute Circuit Breakers**
    *   *Topics:* Step limits, time boundaries, budget tracking, and immediate shutdown codes.
    *   *Resource:* *OWASP Top 10 for LLM Applications (Securing actions)*.
    *   *Assignment:* Implement a circuit-breaker middleware that terminates agent loops when API costs cross $0.05 or execution steps exceed 10.
*   **Day 74: Transaction Boundaries & Rollback States**
    *   *Topics:* ACID properties in agent states, transactional databases, and recovering from file-system errors.
    *   *Reading:* *Designing Data-Intensive Applications*, Chapter 7 (Transactions).
    *   *Assignment:* Create an agent that updates a database table but performs a full rollback if a subsequent tool call fails.
*   **Day 75: Unit-Testing Non-Deterministic Workflows**
    *   *Topics:* Seeding outputs, fuzzy matching, asserting step counts, and mock testing.
    *   *Resource:* *Mattpocock/skills - Fuzzy Testing templates*.
    *   *Assignment:* Build a PyTest suite that executes an agent 10 times and asserts that it retrieves the correct resource at least 9 times.
*   **Day 76: Real-Time State Tracing Dashboards**
    *   *Topics:* Streaming event frames, UI render logs, and tracing tools (LangSmith, Phoenix).
    *   *Resource:* *Dave Ebbelaar's Tracing Guides*.
    *   *Assignment:* Integrate Phoenix or LangSmith tracking into your agent workflow and inspect step executions.
*   **Day 77: Scaling High-Throughput Agentic Backends**
    *   *Topics:* Thread pools, database connections, and load balancing.
    *   *Resource:* *FSDL Operational Scale chapters*.
    *   *Assignment:* Configure Gunicorn and Uvicorn workers to serve your agent backend on 4 concurrent CPU cores.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Measure and catalog latency differences in local agent loops when running on hardware vs. cloud instances.
*   **🛠️ Weekend Lab 11 (4:00 PM - 9:30 PM):** Create a self-correcting Python script execution agent that takes a coding task, runs a test suite, parses exceptions, and fixes its own code.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Loop Engineering: How to Stop Prompting and Start Looping Your AI."*

---

## ⚖️ Phase 4: Evals, Guardrails, & Production Fine-Tuning (Days 78–91)
*Focus: Implementing rigorous quantitative evaluations, building input/output guardrail gateways, compiling fine-tuning datasets, and training custom adapters.*

### Week 12 (Days 78–84): Automated Evaluations & Policy Guardrails
*   **Day 78: Shift from Vibes to Metrics**
    *   *Topics:* Objective performance measurements, regression testing, and creating evaluation harnesses.
    *   *Reading:* *Build Evals and Guardrails*, Section 1.
    *   *Assignment:* List 5 specific failure modes in your tutoring chatbot and draft evaluation metrics for each.
*   **Day 79: Implementing LLM-as-a-Judge Scorer**
    *   *Topics:* Rubrics, scoring scales (1-5), and prompt design for evaluator models.
    *   *Reading:* *Build Evals and Guardrails*, Section 1.2 & 1.3.
    *   *Assignment:* Code an LLM judge using GPT-4o-mini that scores student responses on conceptual accuracy against a rubric.
*   **Day 80: Building Automated Eval Runners**
    *   *Topics:* Thread pool execution, data parsing, exporting markdown scores, and logging bad outputs.
    *   *Reading:* *Build Evals and Guardrails*, Section 1.4.
    *   *Assignment:* Build an evaluation script that runs your agent over a 20-row Golden Dataset, computes percentage accuracy, and lists failures in a text file.
*   **Day 81: Coding Input Guardrails**
    *   *Topics:* Prompt injection detection, PII extraction, toxicity filtering, and input length constraints.
    *   *Reading:* *Build Evals and Guardrails*, Section 2.2.
    *   *Assignment:* Write a regex and classifier system that intercepts user prompts, blocking PII (emails/phones) and injection markers.
*   **Day 82: Coding Output Guardrails**
    *   *Topics:* Structured schema validations (Pydantic), factual hallucination checks, and brand tone enforcement.
    *   *Reading:* *Build Evals and Guardrails*, Section 2.2.
    *   *Assignment:* Code an output interceptor that validates JSON responses against Pydantic model configurations, re-querying the LLM on failures.
*   **Day 83: Securing Applications with OWASP Top 10 Standards**
    *   *Topics:* Security frameworks, rate limits, allow-listing, and input sanitization.
    *   *Resource:* *OWASP Top 10 for LLM Applications (LLM01, LLM06, LLM07)*.
    *   *Assignment:* Perform a secure code review on your FastAPI backend, addressing all vector database filter injection vulnerabilities.
*   **Day 84: Guardrail Latency & False Positive Optimizations**
    *   *Topics:* Caching filter results, measuring latency overhead, and tuning decision thresholds.
    *   *Reading:* *Build Evals and Guardrails*, Section 2.3 & 2.4.
    *   *Assignment:* Profile your API response time with vs. without guardrails, documenting the cost in milliseconds.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Test your Educational Golden Dataset against safety vulnerabilities and prompt injections. Log vulnerability rates.
*   **🛠️ Weekend Lab 12 (4:00 PM - 9:30 PM):** Implement a complete secure Guardrail Gateway API that sits in front of your LLM connections, filtering, validating, and logging safety metrics.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Vibe-Free AI: How to Build Automated Evals and Input/Output Guardrails."*

### Week 13 (Days 85–91): Supervised Fine-Tuning (SFT) & Quantization
*   **Day 85: Behavioral Specification Design**
    *   *Topics:* Standardizing tone, establishing output length limits, and enforcing strict refusal rules.
    *   *Reading:* *How to Make a Fine-tune Ready Dataset*, Section 3 (Step 1).
    *   *Assignment:* Write a detailed behavioral specification sheet for a math-tutoring SLM.
*   **Day 86: Structuring Datasets for SFT**
    *   *Topics:* Conversational JSONL schemas, message lists, and chosen/rejected preference profiles.
    *   *Reading:* *How to Make a Fine-tune Ready Dataset*, Section 2.
    *   *Assignment:* Format a set of 10 multi-turn algebraic discussions into the standard OpenAI messages JSONL format.
*   **Day 87: Data Ingestions & Quality Filters**
    *   *Topics:* Filtering out short outliers, removing duplicated text patterns, and cleaning logs.
    *   *Reading:* *How to Make a Fine-tune Ready Dataset*, Section 3 (Step 5).
    *   *Assignment:* Write a Python filter script that scans a candidate dataset, removing examples where answers are shorter than 50 characters or contain syntax errors.
*   **Day 88: Supervised Fine-Tuning Sprints**
    *   *Topics:* AutoTrain CLI, setting learning rate decays, and batch size controls.
    *   *Resource:* *Unsloth and Axolotl trainer guides*.
    *   *Assignment:* Set up and configure an Axolotl YAML training configuration for a 1B Llama model.
*   **Day 89: PEFT Architectures: LoRA & QLoRA**
    *   *Topics:* Low-rank adapters, rank dimensions, alpha scaling factors, and target modules.
    *   *Paper:* *Dettmers et al., "QLoRA: Efficient Finetuning of Quantized LLMs"*.
    *   *Assignment:* Write a Python PEFT configuration block setting target modules to target all linear layers with rank 16.
*   **Day 90: Model Quantization Formats**
    *   *Topics:* FP16 vs. INT8/INT4 weights, GGUF/AWQ compilation, and local CPU executions.
    *   *Resource:* *Hugging Face quantization docs*.
    *   *Assignment:* Use `llama.cpp` tools to compile a local 3B model into a 4-bit GGUF format.
*   **Day 91: Quantifying Model Regressions & Overfitting**
    *   *Topics:* Catastrophic forgetting, benchmark evaluations, and calculating validation loss curves.
    *   *Reading:* *How to Make a Fine-tune Ready Dataset*, Section 5 & 6.
    *   *Assignment:* Compare the fine-tuned model's success rate on general trivia vs. your math benchmark to measure general knowledge decay.
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Read and summarize frontier guides on Direct Preference Optimization (DPO). Map DPO steps in your research notes.
*   **🛠️ Weekend Lab 13 (4:00 PM - 9:30 PM):** Fine-tune a 1B/3B parameter SLM using QLoRA via Unsloth on 500 clean instructional logs, compile to GGUF, and run it locally.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"How to Train Your Own Local Small Language Model (SLM) on Custom Data."*

---

## 🚀 Phase 5: Advanced Ops & Capstone Showcases (Days 92–100)
*Focus: Engineering self-evolving semantic routers, configuring production scale monitoring, and presenting the final educational AI agent.*

### Week 14 (Days 92–100): Advanced Ops & Capstone Showcases
*   **Day 92: Self-Evolving Semantic Routers**
    *   *Topics:* Vector categorization of inputs, dynamic routing to specialized models or prompts, and routing latency.
    *   *Resource:* *LiteLLM router guidelines*.
    *   *Assignment:* Code a semantic router that routes coding prompts to a coding model and algebra prompts to a math model.
*   **Day 93: Log Analysis & Reinforcement Feedback Loops**
    *   *Topics:* Capturing production logs, parsing user corrections, and tagging drift.
    *   *Reading:* *Why Dataset is Important*, Stage 5 Stage 6.
    *   *Assignment:* Write an automated pipeline that extracts user negative thumbs-down interactions and packages them as evaluation candidates.
*   **Day 94: Real-Time Monitoring & Metric Dashboards**
    *   *Topics:* Prometheus alerts, Grafana dashboard setups, tracking token latency, and error counts.
    *   *Resource:* *Full Stack Deep Learning (FSDL) - Monitoring patterns*.
    *   *Assignment:* Configure a mock Prometheus metrics exporter from your FastAPI server logging request rates.
*   **Day 95: Complete System Audits & Pre-flight Checks**
    *   *Topics:* Security sweeps, schema matching, checking rate limiter tolerances, and final eval runs.
    *   *Reading:* *Build Evals and Guardrails*, Part 3 (Putting them together).
    *   *Assignment:* Run your master eval suite on the finalized unified pipeline, export a PDF benchmark report.
*   **Day 96: Capstone Showcase: Preparing Repositories & Demos**
    *   *Topics:* Writing standard READMEs, packaging environment configurations, and recording step-by-step videos.
    *   *Resource:* *Vibe Coding Showcases (OBRosewell YouTube)*.
    *   *Assignment:* Refactor your master project code, add clean markdown docstrings, and write a detailed repository setup guide.
*   **Day 97: Capstone Showcase: Final Local Launch**
    *   *Topics:* Docker deployment, checking database persistence, and reviewing latency scales.
    *   *Resource:* *Dave Ebbelaar's Deployment playlists*.
    *   *Assignment:* Run the fully compiled container on your local machine and record a successful 5-minute trace demonstration.
*   **Day 98: Research Paper Polish & Formatting Pass**
    *   *Topics:* Typesetting reviews, generating references citations, formatting bibliography, and checking PDF output.
    *   *Guide:* *Research Paper Writing Guide, Section 8*.
    *   *Assignment:* Review and format your LaTeX files inside Overleaf, resolving all compiling warnings.
*   **Day 99: Publishing Code & Artifacts**
    *   *Topics:* Public repository configurations, supplementary dataset releases, and writing release tags.
    *   *Guide:* *Research Paper Writing Guide, Section 11*.
    *   *Assignment:* Push the finalized reproducible evaluation dataset and optimization pipeline code to GitHub.
*   **Day 100: Grand Graduation & Target Submissions**
    *   *Topics:* Submission submissions, slide creation, and sharing on LinkedIn.
    *   *Reading:* *Research Paper Writing Guide, Section 9 & 10*.
    *   *Assignment:* Publish a comprehensive LinkedIn summary about your 100-day journey and link your GitHub repositories!
*   **🔬 Nightly Research (11:30 PM - 2:00 AM):** Select target workshop venues (arXiv, short papers) and compile your final submission packages in Overleaf.
*   **🛠️ Weekend Lab 14 (4:00 PM - 9:30 PM):** Launch your finalized unified system—the Autonomous Learning Agent Capstone.
*   **🎥 Weekend YouTube (11:00 AM - 4:00 PM):** *"Building and Deploying a Fully Stateful, Secure Multi-Agent Educational Platform."*
