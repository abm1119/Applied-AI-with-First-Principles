# How to Validate an AI Idea
**Curriculum Guide — Module 2.1**  
**Purpose:** Stop building the wrong thing. Validate before you write serious code.

---

## 1. Why Most AI Ideas Fail

Most AI projects die for one of these reasons:

- The problem does not actually need AI
- The problem is real but the data does not exist or is too expensive
- The idea only works in a demo, not in the real distribution of users
- No one is willing to pay or change behavior for the solution
- Evaluation is impossible or too expensive

Validation exists to kill bad ideas early and strengthen good ones.

---

## 2. The Validation Framework (5 Layers)

Run every idea through these five layers in order.  
Stop if it fails a layer.

### Layer 1 — Problem Reality Check
Ask:

- Who has this problem today?
- How are they solving it right now (even if the solution is bad)?
- How often does the problem occur?
- What is the cost of the current solution (time, money, frustration)?

**Pass criteria:** You can name real people or companies who feel pain weekly or daily.

**Fail criteria:** “Everyone could use this” or “It would be cool if…”.

### Layer 2 — AI Necessity Test
Ask:

- Can this be solved with normal software + rules + search?
- Does the core value come from language understanding, generation, reasoning, or perception?
- Would a simpler non-AI version still be useful?

**Pass criteria:** The hard part of the problem genuinely requires probabilistic models.

**Fail criteria:** You are using an LLM because it is trendy.

### Layer 3 — Data Feasibility
Ask:

- What data do I need at inference time?
- What data do I need for evaluation?
- What data would I need if I later fine-tune?
- Is that data accessible, legal, and affordable?

**Pass criteria:** You can describe a realistic path to get the necessary data.

### Layer 4 — Evaluation Possibility
Ask:

- How will I know if the system is good?
- Can I create a small golden set of examples?
- Is there an automatic metric, or do I need human judgment?
- Can I measure improvement over a baseline?

**Pass criteria:** You can define at least a crude but honest evaluation method in the first two weeks.

### Layer 5 — Distribution & Willingness to Use
Ask:

- Who will actually use this regularly?
- What behavior change is required?
- Is there a clear trigger (when do they open the tool)?
- Is there a path to payment or strong internal adoption?

**Pass criteria:** You can describe a specific user and a specific moment they would reach for the product.

---

## 3. Practical Validation Process (7–14 days)

### Day 1–2: Write the Idea Card
One page maximum:

- Problem statement
- Target user
- Current alternative
- Proposed AI solution (1–2 sentences)
- Success metric (even if rough)

### Day 3–5: Talk to 5–8 real people
Not friends who will be nice.  
People who currently feel the pain.

Questions to ask:
- Walk me through the last time this problem happened.
- What did you do?
- What was most annoying?
- If a tool existed that did X, would you try it? Why / why not?

### Day 6–8: Build the smallest possible test
Options:
- Manual “Wizard of Oz” prototype (you pretend to be the AI)
- Extremely narrow scripted demo
- Paper prototype + real user reaction

Goal: See if the core magic is actually valuable.

### Day 9–12: Create a tiny Golden Set
10–30 high-quality examples of input → desired output.  
This becomes your first evaluation set.

### Day 13–14: Decision
- Kill
- Pivot
- Continue with clear next milestone

---

## 4. Red Flags (Kill Signals)

- You cannot find 5 people who currently have the problem
- The only data source is “we will scrape the internet”
- Evaluation requires expert humans for every single output and you have no budget
- The idea only works if the model is perfect
- You are more excited about the technology than the user’s pain

---

## 5. Green Flags (Strong Ideas)

- Users already pay money or spend significant time on a worse solution
- You can create a small but high-quality evaluation set quickly
- The AI part is narrow and well-scoped
- There is a clear feedback loop (user can correct or rate the output)
- You can ship a useful non-AI version first and add AI later

---

## 6. Output of Validation

At the end you should have:

1. A clear one-page Idea Card
2. Notes from real user conversations
3. A small Golden Dataset (even 15 examples)
4. A written decision: Kill / Pivot / Proceed
5. The first milestone if you proceed (usually MVP-1)

---

## 7. Relationship to the Rest of the Curriculum

- This guide comes before serious PRD writing and before building.
- The Golden Dataset you create here feeds directly into later RAG and fine-tuning work.
- Evaluation thinking started here becomes the foundation for the full Evals & Guardrails module.

**Rule:**  
No significant engineering effort until the idea has passed at least Layers 1–4.

**Tips**
- When you make your Landing Page, Just post on Social media ... and wait for the feedback.
- Use the `prd-validation-coach.skill` to Validate and Market the idea! 