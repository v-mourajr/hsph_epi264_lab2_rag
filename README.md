<img src="./images/hsph.png" alt="hsph Logo" width="400"><br>

# Lab 2 — Retrieval-Augmented Generation (RAG)  
### EPI 264 — Advanced Epidemiology of Aging

---

## Case Study Continuation  
**Post-Operative Benzodiazepines, Dementia, and Mortality**

In Lab 1, you:

- Built a structured dementia phenotype
- Validated it against a physician gold standard
- Observed sensitivity and specificity limitations

Now we ask:

> Can we improve dementia detection using clinical notes?

---

## Why RAG?

Dementia and cognitive concerns are often:
- Undercoded in diagnosis tables
- Documented only in narrative notes
- Described using non-standard language

Retrieval-Augmented Generation (RAG) allows us to:

1. Retrieve relevant notes for a patient
2. Provide those notes as context to an LLM
3. Ask the model to reason about cognitive status

---

## Objectives of This Lab

You will:

1. Load cleaned notes from Lab 6
2. Create text embeddings
3. Build a simple retrieval index
4. Implement a RAG prompt to classify dementia
5. Compare RAG classification vs structured phenotype
6. Evaluate sensitivity/specificity against gold standard

---

## Deliverables

1. RAG-based dementia classification
2. Comparison table: Structured vs RAG vs Gold
3. Brief interpretation:
   - Did RAG recover false negatives?
   - What new biases might RAG introduce?