# AI Engineering Master Resource Directory (v2)

This master directory contains highly curated, top-tier, and industry-standard resources mapped directly to your 100-Day Applied AI Curriculum. It integrates your favorite educational channels, textbooks, frontier research papers, developer consoles, and academic tools.

---

## 1. Books (High-Quality, Comprehensive & Available Online)
*   **[Understanding Deep Learning](https://udlbook.github.io/udlbook/)** by Simon J.D. Prince (2023)
    *   *Syllabus Sync:* Read **Chapter 14 (Transformers)**, **Chapter 18 (Diffusion Models)**, and **Chapter 19 (Reinforcement Learning)**.
    *   *Why it matters:* Visualizes deep learning concepts with zero mathematical hand-waving. Best resource for diffusion noise grids and self-attention tensor mechanics.
*   **[Speech and Language Processing (3rd ed. Draft)](https://web.stanford.edu/~jurafsky/slp3/)** by Dan Jurafsky and James H. Martin (2024 draft)
    *   *Syllabus Sync:* Read **Chapter 9 (RNNs & LSTMs)**, **Chapter 10 (Transformers & Pretraining)**, and **Chapter 11 (Fine-Tuning & Prompting)**.
    *   *Why it matters:* The absolute bible of NLP. Mandatory background reading for your 8-week educational Small Language Model (SLM) paper's related work section.
*   **[Dive into Deep Learning (D2L)](https://d2l.ai/)** by Aston Zhang, Zack C. Lipton, Mu Li, and Alexander J. Smola
    *   *Syllabus Sync:* Mapped to Phase 4 (SFT, Quantization, and Optimization).
    *   *Why it matters:* Features fully interactive multi-framework code blocks (PyTorch, JAX, NumPy) demonstrating layer configurations, learning rate schedules, and cross-entropy calculations.
*   **[Systems Thinking: Managing Chaos and Complexity (3rd ed.)](https://www.sciencedirect.com/book/99780123851598/systems-thinking)** by Jamshid Gharajedaghi
    *   *Syllabus Sync:* Mapped to Week 10 (Multi-Agent Systems) and Week 11 (Loop Engineering).
    *   *Why it matters:* Essential for understanding feedback loops, system dynamics, and emergent behaviors in multi-agent networks and supervisor routers.
*   **[Patterns of Application Development Using AI](https://github.com/miztiik/patterns-of-application-development-using-ai)** by Miztiik (Open Source Book)
    *   *Syllabus Sync:* Mapped to Week 5 (FastAPI Backend Design) and Week 8 (Context & Memory Engineering).
    *   *Why it matters:* A highly practical pattern-book mapping how to scale session caches, document databases, and vector buffers.
*   **[Designing Data-Intensive Applications (DDIA)](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781491903063/)** by Martin Kleppmann
    *   *Syllabus Sync:* Mapped to Week 5 (Database design, SQL vs NoSQL, and transactions).
    *   *Why it matters:* Explains database durability, transaction boundaries, index caching, and write-ahead logs—vital for scaling persistent agent states.

---

## 2. Official Documentation & References
*   **[Model Context Protocol (MCP) Official Docs](https://modelcontextprotocol.io/)** (Anthropic)
    *   *Syllabus Sync:* Read the **Protocol Specification**, **Quickstart for Python SDK**, and **Exposing Resources & Tools Guide** in Week 6.
*   **[OpenAI Developer Platform & API Reference](https://platform.openai.com/docs/)**
    *   *Syllabus Sync:* Study **Structured Outputs (JSON Schemas)**, **Function Calling (Tools)**, and **Developer Console Assistants API**.
*   **[Anthropic Developer Docs & Prompt Library](https://docs.anthropic.com/)**
    *   *Syllabus Sync:* Read the guides on **Prompt Caching**, **XML Tag Formatting**, and **System Prompts**.
*   **[FastAPI Reference Documentation](https://fastapi.tiangolo.com/)**
    *   *Syllabus Sync:* Mapped to Week 5 (asynchronous request handling, middleware development, routing, and Pydantic validation schemas).
*   **[Hugging Face Docs (Transformers & PEFT)](https://huggingface.co/docs)**
    *   *Syllabus Sync:* Read the setup guides for **AutoModelForCausalLM**, **BitsAndBytes Quantization**, and **PEFT (LoRA/QLoRA configuration)** in Week 13.
*   **[LiteLLM API & Proxy Manual](https://docs.litellm.ai/)**
    *   *Syllabus Sync:* Study unified routing and model fallbacks in Week 5 & 6.
*   **[openpyxl Library Manual](https://openpyxl.readthedocs.io/)**
    *   *Syllabus Sync:* Mapped to your local Excel Tracker scripting and data pipeline outputs.

---

## 3. Whitepapers & Frontier Lab Guides
*   **[OpenAI: Prompt Engineering Best Practices](https://platform.openai.com/docs/guides/prompt-engineering)**
    *   *Syllabus Sync:* Detailed techniques for multi-shot prompting, giving the model "time to think" (reasoning paths), and using reference text delimiters.
*   **[Anthropic: Tool Use (Function Calling) Cookbook](https://github.com/anthropics/anthropic-cookbook)**
    *   *Syllabus Sync:* Step-by-step notebooks showcasing how to write schema-compliant tool parameters and handle model validation errors gracefully.
*   **[Google: Gemini Developer Cookbook](https://github.com/google-gemini/gemini-cookbook)**
    *   *Syllabus Sync:* Advanced notebooks demonstrating **Context Caching** and handling extremely long contexts (up to 2 million tokens) for massive literature databases.
*   **[Cohere: LLM University & RAG Optimization Guide](https://cohere.com/llmu)**
    *   *Syllabus Sync:* Core concepts of Dense vs. Sparse retrieval, lexical search, BM25 indexing, and reranking pipelines.

---

## 4. Curated GitHub Repositories (To Star & Study)
*   **[skills-repository (mattpocock/skills)](https://github.com/mattpocock/skills)**
    *   *Syllabus Sync:* Used in Week 4 for structural mock architectures, modular coding, and Interface/Spec-Driven Development.
*   **[Applied AI Cookbooks (techwithram)](https://github.com/techwithram)**
    *   *Syllabus Sync:* Practical implementations of local vector database setups, multi-tenant RAG, and fast model endpoints.
*   **[Awesome-MCP (punkpeye)](https://github.com/punkpeye/awesome-mcp)**
    *   *Syllabus Sync:* Curated directory of community-built Model Context Protocol servers to immediately plug into Desktop Claude.
*   **[ComfyUI-Manager (ltdrdata)](https://github.com/ltdrdata/ComfyUI-Manager)**
    *   *Syllabus Sync:* Fundamental package manager for managing visual models, ControlNets, and custom extension nodes.
*   **[LangGraph (langchain-ai)](https://github.com/langchain-ai/langgraph)**
    *   *Syllabus Sync:* The standard library for compiling stateful, cyclic multi-agent graphs.
*   **[Unsloth (unslothai/unsloth)](https://github.com/unslothai/unsloth)**
    *   *Syllabus Sync:* Enables 2x to 5x faster supervised fine-tuning (SFT) and LoRA generation with 80% less memory usage.

---

## 5. Articles, Blogs & Long-Form Writing
*   **[Lil'Log (lilianweng.github.io/posts)](https://lilianweng.github.io/posts/)** by Lilian Weng (Director of AI Safety, OpenAI)
    *   *Must-Reads:* **"LLM-Powered Autonomous Agents" (2023)** (foundational blueprint for ReAct and tool-use), **"RAG" (2023)**, and **"Prompt Engineering" (2023)**.
*   **[Eugene Yan's Blog (eugeneyan.com)](https://eugeneyan.com/)**
    *   *Must-Reads:* **"Patterns for Building LLM-based Applications"** and **"How to Build and Evaluate a RAG System"**. Excellent focus on operational reliability and avoiding metric-chasing.
*   **[Chip Huyen's Blog (huyenchip.com)](https://huyenchip.com/)**
    *   *Must-Reads:* **"Evaluation of Foundation Models"** and **"Building LLM Applications for Production"**. Essential advice on dataset separation and pipeline latencies.
*   **[LLM-Bento (llm-bento.com)](https://www.llm-bento.com/)**
    *   *Syllabus Sync:* Detailed diagrams of context-window cache mechanics, KV-cache storage, and model serving benchmarks.
*   **[Aman's AI (amanxai.com)](https://amanxai.com/)**
    *   *Syllabus Sync:* Practical guides detailing how to design prompt gateways, manage state in chats, and build localized pipelines.

---

## 6. Major Organisation Guides & Standards
*   **[Full Stack Deep Learning (FSDL)](https://fullstackdeeplearning.com/)**
    *   *Focus:* The ultimate guide on infrastructure setup, cost estimation, CI/CD for ML models, and drift monitoring.
*   **[DataTalksClub: LLM Zoomcamp](https://github.com/DataTalksClub/llm-zoomcamp)**
    *   *Focus:* Hands-on curriculum mapping out search engine construction (Elasticsearch), vector databases (Chroma/Qdrant), and RAG performance measuring.
*   **[OWASP Top 10 for LLM Applications Project](https://owasp.org/www-project-top-10-for-large-language-model-applications/)**
    *   *Focus:* The absolute global standard for securing LLMs. Explains the mechanics, risks, and mitigations of Prompt Injection (LLM01), Data Leakage (LLM06), and Insecure Plugin Design (LLM07).

---

## 7. Crucial Research Papers (Deep Dive List)
*   **Transformer Architectures:**
    *   *"Attention Is All You Need"* (Vaswani et al., 2017) – The paper that started it all. Focus on the scaled dot-product attention formula and multi-head projection layers.
*   **Agentic Loops & Planning:**
    *   *"ReAct: Synergizing Reasoning and Acting in Language Models"* (Yao et al., 2022) – Proved that interleaved thinking and action traces improve logical performance on multi-step tasks.
*   **Adaptation & Fine-Tuning:**
    *   *"LoRA: Low-Rank Adaptation of Large Language Models"* (Hu et al., 2021) – Introduced parameterized adapter weights ($W = W_0 + B A$).
    *   *"QLoRA: Efficient Finetuning of Quantized LLMs"* (Dettmers et al., 2023) – Introduced double-quantized NF4 formats to fit massive training runs on commodity GPUs.
*   **Retrieval Evaluation:**
    *   *"RAGAS: Automated Evaluation of Retrieval Augmented Generation"* (Es et al., 2023) – The seminal paper defining mathematically rigorous formulas for Faithfulness, Answer Relevance, and Context Recall.
*   **Alignment & Preference Optimization:**
    *   *"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"* (Rafailov et al., 2023) – Elided the complex training steps of RLHF by optimizing SFT parameters directly on chosen/rejected dataset logs.

---

## 8. Newsletters, Sites & Communities
*   **[DAIR.AI (dair.ai)](https://dair.ai/)**: Community-driven summaries of the latest research papers and engineering libraries. Great visual explainers.
*   **[The Batch (DeepLearning.AI)](https://www.deeplearning.ai/the-batch/)**: Andrew Ng's weekly update. Highly readable digests of frontier releases and deployment case studies.
*   **[Alpha Signal (alphasignal.ai)](https://alphasignal.ai/)**: Highly technical newsletter curating the most active repos, papers, and libraries on GitHub and ArXiv every week.

---

## 9. Interactive Tools, Sites & Libraries
*   **[ArXiv Sanity Preserver](http://www.arxiv-sanity.com/)**: Essential search and recommendation client built to surface non-trivial ML papers.
*   **[Excalidraw](https://excalidraw.com/)**: Excellent minimalist sketching board for drawing ERDs, pipeline architectures, and agent state transitions.
*   **[Hugging Face Spaces](https://huggingface.co/spaces)**: Search and interact with live implementations of new models (e.g., Flux Schnell, Wan Animate, and SkyReels).

---

## 10. Free & Underrated Courses
*   **[BuildWithHussain (YouTube)](https://www.youtube.com/@BuildWithHussain)**: Invaluable visual tutorials detailing how to design custom tool calling setups, build MCP servers in Python, and write stateful agent loops.
*   **[Dave Ebbelaar (YouTube)](https://www.youtube.com/@daveebbelaar)**: Highly hands-on tutorials building production-ready RAG setups, semantic search APIs, and database persistencies.
*   **[OBRosewell (YouTube)](https://www.youtube.com/@OBRosewell)**: Deep-dives into rapid vibe coding, outlining how to build robust, spec-driven MVPs in minutes using cursor prompts and structural tests.
*   **[Chai aur Code (YouTube)](https://www.youtube.com/@chaiaurcode)**: Masterful programming courses covering backend engineering, asynchronous queues, database connectivity, and environment management.

---

## 11. Bonus Academic Toolchain (For Your Research Paper)
*   **[Zotero Reference Manager](https://www.zotero.org/)**: The ultimate bibliography collector. Install the **Zotero Connector** for Chrome/Firefox to save research papers with a single click.
*   **[Better BibTeX for Zotero](https://retorque.re/zotero-better-bibtex/)**: Automates the generation of consistent, clean BibTeX keys (`[AuthorYear]`) and auto-updates your project's `.bib` references file.
*   **[Overleaf Collaborative LaTeX Editor](https://www.overleaf.com/)**: The standard cloud environment for writing, compiling, and editing academic papers in LaTeX. Features hundreds of templates for IEEE, ACM, and NeurIPS.
