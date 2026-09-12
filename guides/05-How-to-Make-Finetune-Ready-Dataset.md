# How to Make a Fine-tune Ready Dataset
**Curriculum Guide — Module 2.6 + 2.9**  
**Purpose:** Prepare high-quality data that actually improves a model instead of making it worse.

---

## 1. Core Principle

Fine-tuning is not magic.  
It is supervised learning on top of a strong base model.

The model will imitate the patterns in your data — including the bad ones.

Therefore the dataset must be:
- Correct
- Consistent in style and format
- Representative of the target distribution
- Free of unnecessary noise

---

## 2. Main Formats You Will Use

### A. Supervised Fine-Tuning (SFT) Format
```json
{
  "messages": [
    {"role": "system", "content": "..."},
    {"role": "user", "content": "..."},
    {"role": "assistant", "content": "..."}
  ]
}
```
or simpler instruction format:
```json
{
  "instruction": "...",
  "input": "...",
  "output": "..."
}
```

### B. Preference / Ranking Format (for DPO, ORPO, etc.)
```json
{
  "prompt": "...",
  "chosen": "...",
  "rejected": "..."
}
```

### C. Continuation / Completion Format
Less common for chat models, more for specialized tasks.

---

## 3. Step-by-Step Creation Process

### Step 1 — Decide the exact behavior you want
Write a clear behavioral specification:
- Tone
- Length
- Structure
- What to do when uncertain
- What to refuse

This becomes the standard every example must follow.

### Step 2 — Start from your Golden Dataset
Your Golden Dataset is the highest quality seed.
Expand it carefully.

### Step 3 — Generate candidate examples
Sources:
- Human-written (best)
- Strong model generations + heavy human editing
- Real production logs (cleaned and corrected)
- Synthetic data (only with strict filtering)

### Step 4 — Enforce consistency
Check for:
- Same formatting style
- Same level of detail
- Same refusal behavior
- No contradictory answers across the dataset

Inconsistency teaches the model to be inconsistent.

### Step 5 — Filter aggressively
Remove:
- Incorrect answers
- Hallucinated facts
- Overly long or overly short outliers (unless intentional)
- Examples that leak evaluation data
- Toxic or off-brand content

### Step 6 — Split properly
- Training set
- Validation / development set
- Held-out test set (ideally from your Golden Dataset or a strict separate set)

Never tune on the final test set.

### Step 7 — Version and document
Record:
- How the data was created
- Which model versions helped generate it
- Filtering rules applied
- Date and version number

---

## 4. Size Guidelines (Practical)

| Goal | Starting Size | Notes |
|------|---------------|-------|
| Style / tone adaptation | 100–500 | Often enough |
| Domain knowledge injection | 500–3000+ | Quality still matters more |
| Complex new skill | 1000–10000+ | Depends on difficulty |
| Preference tuning | 500–5000 pairs | Chosen/rejected must be clearly different |

More data only helps if it is clean and on-distribution.

---

## 5. Special Considerations

### For RAG + Fine-tuning combination
- Do not fine-tune on knowledge that should stay in the retrieval system unless you have a strong reason.
- Fine-tune for behavior, format, reasoning style, and tool use.
- Keep factual knowledge in RAG when possible (easier to update).

### For Agents
- Include examples of tool calling
- Include examples of recovery from tool errors
- Include examples of when not to call a tool

### For Safety
- Explicitly include refusal examples
- Include borderline cases so the model learns the boundary

---

## 6. Common Mistakes

- Using raw unedited model outputs as training data
- Mixing many different styles in one dataset
- Fine-tuning on the same data you use for final evaluation
- Creating preference pairs where “chosen” and “rejected” are almost the same
- Ignoring the base model’s existing strengths and overwriting them

---

## 7. Quality Checklist Before Training

- [ ] Every example follows the behavioral specification
- [ ] Format is 100% consistent
- [ ] No evaluation data leaked into training
- [ ] Clear train / val / test split
- [ ] Refusal and edge cases are represented
- [ ] Dataset is versioned and documented

---

## 8. Relationship to Other Guides

- Built on top of the **Golden Dataset**
- Often uses cleaned content from the **RAG-Ready** corpus
- Directly enables the **Fine-Tuning Track (2.9)**
- Evaluation of the fine-tuned model uses the same Golden Dataset + Evals framework

**Final Rule:**  
If you are not willing to read and defend every example in your fine-tuning set, the set is not ready.
