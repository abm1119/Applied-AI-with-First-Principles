# How to Make a RAG-Ready Dataset
**Curriculum Guide — Module 2.6**  
**Purpose:** Turn raw documents into a clean, retrieval-optimized knowledge base.

---

## 1. What “RAG-Ready” Actually Means

A RAG-Ready dataset is not just a folder of PDFs.  
It is a collection of chunks that are:

- Semantically coherent
- Properly sized for the embedding model
- Enriched with useful metadata
- Cleaned of noise
- Easy to update and version

Bad chunking or missing metadata is the #1 reason RAG systems feel stupid.

---

## 2. The Full Pipeline

```
Raw Sources → Cleaning → Chunking → Metadata → Embedding → Vector Store → Evaluation
```

---

## 3. Step-by-Step Process

### Step 1 — Collect and Inventory Sources
List every source:
- Product docs
- Notion / Confluence
- PDFs
- Support tickets (cleaned)
- Policies
- Code (if relevant)

Record: source name, owner, update frequency, license/sensitivity.

### Step 2 — Clean the Text
Remove or fix:
- Headers, footers, page numbers
- Navigation menus
- Duplicate content
- Broken encoding
- Irrelevant sections (legal boilerplate if not needed)

Keep the meaning intact. Do not over-summarize yet.

### Step 3 — Choose a Chunking Strategy
Common strategies:

| Strategy | Best for | Notes |
|----------|----------|-------|
| Fixed size (with overlap) | General docs | Simple, good starting point |
| Semantic / paragraph | Well-structured text | Better coherence |
| Document structure aware | Technical docs, manuals | Respect headings |
| Parent-child / hierarchical | Long documents | Retrieve small + expand context |

Practical starting point:
- 300–800 tokens per chunk
- 10–20% overlap
- Respect markdown/header boundaries when possible

### Step 4 — Attach Rich Metadata
Minimum useful metadata:
- source
- title / section
- url or document id
- last_updated
- product / category
- access level (if needed)

Advanced metadata:
- keywords
- summary of the chunk
- hypothetical questions the chunk answers

Metadata enables filtering and better ranking later.

### Step 5 — Create Retrieval Evaluation Questions
From your Golden Dataset (or new questions):
- Write questions that should retrieve specific chunks
- Record which chunk(s) are the correct ones

This becomes your retrieval test set.

### Step 6 — Embed and Load
- Choose an embedding model (start with a strong general one)
- Store vectors + metadata in your vector database
- Version the index

### Step 7 — Evaluate Retrieval Quality
Metrics to start with:
- Recall@k (does the right chunk appear in top k?)
- MRR or nDCG if you have ranked relevance
- Manual inspection of failure cases

Fix chunking or metadata based on failures — not by jumping to a bigger model.

---

## 4. Practical Checklist Before You Call It “Ready”

- [ ] Sources are inventoried and cleaned
- [ ] Chunk size and overlap are intentional
- [ ] Every chunk has useful metadata
- [ ] You have at least 30–50 retrieval test questions
- [ ] You can measure Recall@5 or Recall@10
- [ ] You have a process to update documents later

---

## 5. Common Failure Modes

- Chunks that are too small → no context
- Chunks that are too large → diluted embeddings
- No overlap → answers split across boundaries
- Missing metadata → cannot filter by product/date
- Evaluating only generation quality and ignoring retrieval quality

---

## 6. Relationship to Other Guides

- Your **Golden Dataset** questions become the retrieval test set.
- Clean RAG data later becomes a source for **Fine-tune Ready** data if you decide to fine-tune on domain knowledge.
- Retrieval failures feed directly into **Evals & Guardrails**.

---

## 7. Rule of Thumb

Spend more time on cleaning, chunking, and metadata than on choosing the vector database.  
The database is the easy part. The data is the hard part.
