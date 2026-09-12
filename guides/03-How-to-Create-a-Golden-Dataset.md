# How to Create a Golden Dataset
**Curriculum Guide — Module 2.6**  
**Purpose:** Build the highest-leverage artifact in applied AI — a small, trusted set of examples that defines “correct” behavior.

---

## 1. What is a Golden Dataset?

A Golden Dataset is a carefully curated collection of input → expected output pairs that you treat as the source of truth.

It is used for:

- Evaluating any system (prompted, RAG, agent, fine-tuned)
- Regression testing when you change prompts, models, or retrieval
- Guiding fine-tuning and preference data creation
- Aligning the team on what “good” looks like

It is usually small at the beginning (20–200 examples) and grows over time.

---

## 2. Properties of a Good Golden Dataset

| Property | Meaning | Why it matters |
|----------|---------|----------------|
| Correct | Outputs are actually what you want | Garbage evaluation is worse than no evaluation |
| Diverse | Covers normal cases, edge cases, and failure modes | Prevents overfitting to easy examples |
| Realistic | Looks like real user inputs | Lab performance must transfer |
| Unambiguous | Clear what the right answer is | Disagreements destroy trust in metrics |
| Versioned | You know exactly which version you are using | Reproducibility |
| Separated | Never used for training/fine-tuning | Prevents data leakage |

---

## 3. Step-by-Step Creation Process

### Step 1 — Define the task clearly
Write one paragraph:
- What is the input?
- What should the output contain?
- What should it never do?

### Step 2 — Collect real or realistic inputs
Sources (in order of preference):
1. Real user queries (anonymized)
2. Support tickets / logs
3. Manually written examples that mirror real distribution
4. Synthetic examples (only after you have real ones)

Aim for the actual language and messiness of users.

### Step 3 — Create high-quality outputs
For each input, produce the ideal output.
- Do it yourself first
- Or have a domain expert do it
- Or generate with a strong model and then heavily edit

Never accept raw model output as golden without human review.

### Step 4 — Cover the important categories
Explicitly include:

- Happy path (normal, common cases)
- Edge cases (long input, short input, ambiguous, multilingual, etc.)
- Adversarial / abuse cases (if relevant)
- Cases where the correct behavior is “I don’t know” or refusal

### Step 5 — Add metadata
Useful fields:
- id
- input
- ideal_output
- category / tag
- difficulty
- source
- notes
- date_added

### Step 6 — Review and freeze a version
Have at least one other person review a sample.  
Then freeze version 1.0 and start using it for evaluation.

---

## 4. Recommended Starting Size

| Stage | Size | Goal |
|-------|------|------|
| Idea validation | 10–30 | See if the core idea works |
| First serious MVP | 50–100 | Basic regression + development |
| Production system | 200–1000+ | Reliable measurement + drift detection |

Start small and high-quality. Grow later.

---

## 5. Format Example (JSONL)

```json
{"id": "001", "input": "How do I reset my password?", "ideal_output": "Go to Settings → Security → Reset Password. You will receive an email with a link valid for 30 minutes.", "category": "account", "difficulty": "easy"}
{"id": "002", "input": "My package says delivered but I don't have it", "ideal_output": "I'm sorry about that. Please check with neighbours and your building reception first. If still missing, open a claim here: [link]. I can also escalate to support if you want.", "category": "shipping", "difficulty": "medium"}
```

---

## 6. Common Mistakes

- Making all examples too clean and polite
- Only including cases the current system already handles well
- Using the same examples for development and final evaluation
- Never updating the golden set as the product evolves
- Treating model-generated answers as ground truth without review

---

## 7. How the Golden Dataset is Used Later

- **Evals**: Score new prompts, models, or RAG pipelines against it
- **RAG**: Turn questions from the golden set into retrieval test cases
- **Fine-tuning**: Expand it into training data (carefully, with separation)
- **Guardrails**: Extract bad behaviors you want to block
- **Monitoring**: Compare production outputs against golden-style expectations

---

## 8. Practical Rule

Create the first version of your Golden Dataset **before** you invest heavily in complex architecture.

It is cheaper to build 30 excellent examples than to debug a system with no definition of “correct.”
