# Build Evals and Guardrails
**Curriculum Guide — Module 2.7**  
**Purpose:** Make your AI systems measurable and safe enough to put in front of real users.

---

## Part 1 — Evaluation (Evals)

### 1.1 Why Evals Come Before Fancy Architecture

You cannot improve what you cannot measure.  
Without evals you are developing by vibes.

Good evals let you answer:
- Is version B actually better than version A?
- Did the new prompt regress on important cases?
- Is the agent getting worse as we add tools?
- Are we ready to ship?

### 1.2 Types of Evaluation

| Type | Description | When to use |
|------|-------------|-------------|
| Golden Dataset eval | Score against trusted input-output pairs | Always (baseline) |
| LLM-as-Judge | Use a strong model to score outputs | Scalable subjective quality |
| Human eval | Real people rate outputs | High-stakes or nuanced tasks |
| Task success metrics | Did the user achieve the goal? | Product-level |
| Retrieval metrics | Recall, precision of RAG | Any RAG system |
| Safety / policy eval | Did it refuse correctly? | All user-facing systems |
| Online / production eval | Real traffic + feedback | After launch |

### 1.3 Building Your First Eval Suite

1. Start with your **Golden Dataset**
2. Define scoring methods:
   - Exact match (rare)
   - Key point coverage
   - Rubric-based scoring (1–5)
   - Binary pass/fail on critical rules
3. Automate as much as possible
4. Keep a small manual review loop
5. Run the suite on every significant change

### 1.4 Practical Eval Architecture

```
Input → System under test → Output
                ↓
        Scorer (code + LLM judge + rules)
                ↓
        Metrics + Failure examples
                ↓
        Dashboard / report
```

Track:
- Overall score
- Score by category
- Worst failures
- Trend over time

### 1.5 Common Eval Mistakes

- Only testing happy paths
- Using the same data for development and final reporting
- Changing the judge prompt and thinking the model improved
- Ignoring retrieval quality when evaluating RAG
- No regression tests

---

## Part 2 — Guardrails

### 2.1 What Guardrails Actually Are

Guardrails are deterministic or semi-deterministic controls that sit around the model to enforce rules the model itself cannot be fully trusted with.

They protect against:
- Harmful or disallowed content
- Prompt injection
- Data leakage
- Hallucinated actions (in agents)
- Brand or policy violations
- Cost / latency explosions

### 2.2 Layers of Guardrails

**Input Guardrails**
- Profanity / toxicity filters
- Prompt injection detection
- PII detection
- Topic allow/deny lists
- Length and rate limits

**Output Guardrails**
- Content policy classifiers
- Hallucination checks (against retrieved context)
- Format validation (JSON schema, etc.)
- Refusal enforcement
- Brand voice checks

**System / Agent Guardrails**
- Tool call allow-lists
- Maximum steps / recursion limits
- Human-in-the-loop triggers
- Budget limits (tokens, money)
- Sandboxing of code execution

### 2.3 Implementation Approaches

1. **Rules & Regex** — fast, cheap, limited
2. **Classifiers** — dedicated models for toxicity, injection, etc.
3. **LLM checks** — flexible but need careful prompting and cost control
4. **Structured output + validation** — Pydantic / JSON schema
5. **External policy engines** — for enterprise settings

Best practice: combine several layers. Never rely on the main model alone.

### 2.4 Guardrail Design Process

1. List the concrete risks for your product
2. Rank them by severity and likelihood
3. Choose the lightest control that adequately reduces the risk
4. Measure false positive rate (very important for user experience)
5. Log every guardrail trigger for later analysis
6. Review and update regularly

---

## Part 3 — Putting Evals and Guardrails Together

### Recommended Minimum for Any User-Facing System

- Golden Dataset of at least 50–100 examples
- Automated eval suite that runs on every prompt/model change
- Basic input filtering (injection + PII + length)
- Output format validation
- Clear refusal behavior tested in the golden set
- Logging of both normal and blocked requests
- Simple dashboard or even a weekly manual review of failures

### For Agents (Higher Bar)

- Everything above
- Maximum step limits
- Tool allow-listing
- Evaluation of multi-step trajectories (not just final answer)
- Human approval for high-impact actions
- Budget circuit breakers

---

## 4. Relationship to the Curriculum

- Golden Dataset (Guide 03) is the foundation of evals
- RAG-Ready data quality directly affects retrieval evals
- Fine-tune Ready data must be evaluated with the same suite
- Harness Engineering and Loop Engineering depend on strong evals
- You cannot do reliable self-evolving systems without measurement

---

## 5. Practical Rule

Ship with imperfect features.  
Do not ship without measurement and basic guardrails.

Evals tell you whether you are going in the right direction.  
Guardrails keep the system from causing damage while you improve it.
