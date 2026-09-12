# Academic Research Paper Progress Log & Daily Sprint Tracker
## Topic: Optimizing SLMs in Educational Agentic Workflows

Welcome to your structured 8-week research sprint log! This tracker is customized to fit your exact daily routine [68]:
*   **Weekdays (Monday to Friday):** 11:30 PM – 2:00 AM (2.5 hours of pure focus on reading, writing, and experiment logging) [68].
*   **Weekends (Saturday and Sunday):** 2–4 hours allocated from your 4:00 PM – 9:30 PM Learn & Build block [56, 68].

Use this log daily to track your milestones, document your data, log experiment results, and stay on track [58, 59].

---

## 📅 The 8-Week Research Sprint Roadmap

```
Week 1–2: Lit Survey & Scope → Week 3: Problem Design → Week 4–5: Code & Run Tests → Week 6: Write Core → Week 7: Polish Draft → Week 8: Publish & Package
```

---

## 📓 Week 1 & 2: Foundation, Scope & Literature Survey
*   **Goal:** Build a database of 25–40 papers, finalize research questions, set up LaTeX, and draft Section 3 (Related Work) [56, 60].
*   **Hours Target:** 30 hours total (2.5 hours/day weekdays + 2.5 hours/day weekends) [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 1 (Mon):** Create folder structure `/research-paper/` and set up Zotero library and browser extension [59, 67].
*   [ ] **Day 2 (Tue):** Write a one-page "Research Idea Card" validating your research question [7, 67].
*   [ ] **Day 3 (Wed):** Formulate exact search queries and find first 10 seed papers on Google Scholar/arXiv [60, 67].
*   [ ] **Day 4 (Thu):** Set up Overleaf and import your target conference LaTeX template [59].
*   [ ] **Day 5 (Fri):** First Pass skim of 10 papers; select 5 for deep reading [60].
*   [ ] **Day 6–7 (Sat–Sun):** Spend 4 hours deep reading. Capture literature notes (Question, Method, Findings, Gaps) [60].
*   [ ] **Day 8 (Mon):** Run forward/backward citation chaining on the top 2 seed papers to find 10 more papers [60].
*   [ ] **Day 9 (Tue):** Deep read 3 papers on local SLM optimizations (Phi-3, Llama-3-8B) [60, 65].
*   [ ] **Day 10 (Wed):** Deep read 3 papers on agentic loop architectures (ReAct, state machines) [71].
*   [ ] **Day 11 (Thu):** Deep read 3 papers on generative pedagogical tutoring systems [1, 60].
*   [ ] **Day 12 (Fri):** Cluster your 25–40 collected papers into 3 distinct themes [60].
*   [ ] **Day 13–14 (Sat–Sun):** Draft Section 3: Related Work in LaTeX. Cite your papers using BibTeX keys [56, 59].

### Deliverables Checklist
*   [ ] Private Private privée GitHub repository initialized with private privadas Private privado credentials [59].
*   [ ] Zotero collection populated with 25–40 papers with attached citation notes [56, 60].
*   [ ] Overleaf project created with compiling BibTeX bibliography [59].
*   [ ] Compiling draft of "Section 3: Related Work" (approx. 2–3 pages) [56, 61].

---

## 📓 Week 3: Problem Formalization & System Design
*   **Goal:** Formulate inputs, outputs, educational objectives, and design the agentic SLM workflow [56].
*   **Hours Target:** 15 hours total [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 15 (Mon):** Define the Input/Output space of your educational agent mathematically ($S$, $C$, $R$, $T$) [1, 54, 71].
*   [ ] **Day 16 (Tue):** Sketch the step-by-step state machine or ReAct loop diagram on paper or draw.io [59, 71].
*   [ ] **Day 17 (Wed):** Outline your SLM optimization pipeline (prompt strategies, routing, formatting) [1, 54, 71].
*   [ ] **Day 18 (Thu):** Define technical metrics (success rate, latency, token cost) and pedagogical metrics [62].
*   [ ] **Day 19 (Fri):** Design the scoring rubrics for your LLM-as-a-Judge evaluation framework [46, 62].
*   [ ] **Day 20–21 (Sat–Sun):** Draft Section 4 (Problem Formulation) and Section 5 (Proposed Approach) in LaTeX [56, 61].

### Deliverables Checklist
*   [ ] Complete system architecture / agent loop diagram (SVG, PNG, or vector) [57, 59].
*   [ ] Mathematical formalization of the problem statement [56, 61].
*   [ ] Fully drafted Section 4 and Section 5 in Overleaf [56, 61].

---

## 📓 Week 4 & 5: Implementation & Experimental Execution
*   **Goal:** Build the agent codebase, construct your Educational Golden Dataset, run SLM vs. LLM benchmark tests, and collect results [57].
*   **Hours Target:** 30 hours total [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 22 (Mon):** Initialize your private private privately private workspace repository code structures [59].
*   [ ] **Day 23 (Tue):** Write the core localized SLM inference class (using Ollama, vLLM, or Hugging Face) [65].
*   [ ] **Day 24 (Wed):** Code the agent's routing system, prompt managers, and tool registry [71].
*   [ ] **Day 25 (Thu):** Build the complete interactive student-agent simulation loop [1, 54, 71].
*   [ ] **Day 26 (Fri):** Run a sanity check on 5 test student queries to ensure the loop doesn't infinite-loop [49, 51].
*   [ ] **Day 27–28 (Sat–Sun):** Build your **Educational Golden Dataset**: Create 50 high-quality tutoring queries and ideal response pairs [62].
*   [ ] **Day 29 (Mon):** Code the automated Evaluation Scorer script (using a strong LLM as a Judge with your rubrics) [46, 62].
*   [ ] **Day 30 (Tue):** Execute your baseline runs (raw, un-optimized SLMs like raw Llama-3-8B) and save logs [57].
*   [ ] **Day 31 (Wed):** Execute optimized SLM runs. Capture latency, step counts, and token counts [62].
*   [ ] **Day 32 (Thu):** Execute frontier LLM runs (GPT-4o or Claude 3.5 Sonnet) to establish the upper bound [54, 57].
*   [ ] **Day 33 (Fri):** Parse raw logs and aggregate metrics into mean, median, and variance values [57].
*   [ ] **Day 34–35 (Sat–Sun):** Plot latency vs. accuracy and cost vs. accuracy charts using Python (Matplotlib/Plotly) [57].

### Deliverables Checklist
*   [ ] Fully functional private privately privadas private privately private private repository code with execution scripts [59].
*   [ ] Completed JSONL file containing the 50-example Educational Golden Dataset [62].
*   [ ] Raw execution CSV/JSON logs detailing every run's latency, token counts, and judge scores [57, 62].
*   [ ] Visual performance charts ready for inclusion in the paper [57].

---

## 📓 Week 6: Results Analysis & Drafting Core Sections
*   **Goal:** Analyze evaluation metrics, do error-analysis on failure runs, and draft Method, Setup, and Results sections [57].
*   **Hours Target:** 15 hours total [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 36 (Mon):** Construct your LaTeX results tables comparing your SLM, baseline SLM, and frontier LLMs [57, 61].
*   [ ] **Day 37 (Tue):** Conduct an Error Analysis: Take the lowest-scoring 10 runs of your SLM and categorize why they failed [46, 65].
*   [ ] **Day 38 (Wed):** Draft Section 6 (Experimental Setup) detailing hardware, models, datasets, and hyperparameters [57, 61, 65].
*   [ ] **Day 39 (Thu):** Draft Section 7 (Results) detailing the numerical comparison, latency analysis, and cost saving [57, 61, 62].
*   [ ] **Day 40 (Fri):** Write up the Qualitative / Pedagogical analysis based on the LLM judge comments [57, 62].
*   [ ] **Day 41–42 (Sat–Sun):** Finalize all LaTeX table structures and make sure figures are properly scaled and referenced [57].

### Deliverables Checklist
*   [ ] Clean LaTeX results table comparing baselines and your model [57, 61].
*   [ ] A structured Qualitative Analysis subsection with selected qualitative examples [57].
*   [ ] Complete Section 6 and Section 7 drafts compiled in Overleaf [57, 61].

---

## 📓 Week 7: Full Draft Integration & Related Work Polish
*   **Goal:** Write Discussion, Limitations, Conclusion, and Introduction sections. Integrate into a unified paper draft [57].
*   **Hours Target:** 15 hours total [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 43 (Mon):** Draft Section 8 (Discussion): Synthesize your findings. What do these numbers actually mean for classrooms? [57, 61]
*   [ ] **Day 44 (Tue):** Draft Section 9 (Limitations & Future Work): Honestly address compute budgets, context constraints, and edge cases [61, 65].
*   [ ] **Day 45 (Wed):** Draft Section 10 (Conclusion) summarizing core findings and implications [57, 61].
*   [ ] **Day 46 (Thu):** Draft Section 2 (Introduction) using the 5-paragraph formula [61, 63].
*   [ ] **Day 47 (Fri):** Draft Section 1 (Abstract) and finalize a strong, concise title [61, 63].
*   [ ] **Day 48–49 (Sat–Sun):** Run the complete compilation. Check transitions and read sections aloud to fix sentence lengths [63].

### Deliverables Checklist
*   [ ] Full compiling LaTeX manuscript (approx. 8–10 pages) containing all 10 standard sections [61].
*   [ ] Claims-Evidence Matrix finalized and cross-verified [63].
*   [ ] First complete PDF draft generated from Overleaf [57, 59].

---

## 📓 Week 8: Polish, Submission Package & Artifacts
*   **Goal:** Final proofreading pass, clean supplementary codebase, and prepare the submission zip package [57].
*   **Hours Target:** 15 hours total [56, 68].

### Daily Sprint Checklist
*   [ ] **Day 50 (Mon):** Verify spelling, math notation consistency, and citation formatting in Overleaf [57, 59].
*   [ ] **Day 51 (Tue):** Clean up repository code, add a reproducible README file, and make the GitHub repo public [59].
*   [ ] **Day 52 (Wed):** Verify your BibTeX file inside Zotero to eliminate double brackets, missing years, or broken authors [59].
*   [ ] **Day 53 (Thu):** Convert your paper draft to a PDF and send it to your mentors or peer reviewers for feedback [57].
*   [ ] **Day 54 (Fri):** Review peer comments and make final surgical adjustments to the manuscript [57].
*   [ ] **Day 55–56 (Sat–Sun):** Compile final source files, build a structured supplementary data zip, and submit [57].

### Deliverables Checklist
*   [ ] Submission-ready PDF manuscript [57].
*   [ ] Publicly accessible, clean GitHub repository with a "Reproducibility Guide" [59].
*   [ ] Standard supplementary material package (prompts, configuration JSONs, anonymized golden evaluations) [57, 62].

---

## 📝 Research Diary & Experiment Logs
*Use this section below to live-document literature ideas, logging experiment parameters, and capture draft thoughts during your 11:30 PM session.*

### 📚 Literature Survey Snippets
| ID | Paper Title | Key Finding | Relevance to My Work |
| :--- | :--- | :--- | :--- |
| *01* | *Example: "ReAct: Synergizing Reasoning and Acting"* | *ReAct pattern combines chain-of-thought with tool search* | *Core workflow structure of our tutoring SLM agent* |
| | | | |

### 🧪 Experiment Tracker
*   **Baseline Model:** `un-optimized-llama-3-8b`
*   **Optimized Model:** `prompt-optimized-quantized-phi-3-medium`
*   **Evaluation Set:** `Educational Golden Dataset v1.0 (50 Examples)`

| Run ID | Model Name | Accuracy (Rubric % ) | Latency (sec) | Cost / 1k Runs ($) | Notes / Error Patterns |
| :--- | :--- | :--- | :--- | :--- | :--- |
| *R01* | *Llama-3-8B* | *68.5%* | *4.2s* | *$0.00 (Local)* | *Struggled with complex educational state transitions* |
| | | | | | |
