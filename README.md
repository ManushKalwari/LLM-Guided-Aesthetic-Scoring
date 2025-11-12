# Learning an Aesthetic Reward Function Using LLM-Guided Optimization

This notebook explores how large language models can be used to design interpretable aesthetic reward functions — heuristics that approximate human aesthetic judgment.

We prompt an LLM to iteratively refine a Python scoring function that combines *human-annotated visual attributes* such as *composition, lighting, subject focus, and color palette.*
The model learns weighting schemes that correlate strongly with human aesthetic preference, achieving a test *Spearman correlation of ρ ≈ 0.82*.

---

### Overview
We designed a reasoning-driven optimization loop where the LLM:
1. Analyzes distributions of visual attributes from annotated data.  
2. Iteratively proposes and tests new scoring functions.  
3. Evaluates each version against human scores using correlation metrics.  
4. Refines the heuristic until it aligns with aesthetic judgment.

This process produces a reward function that generalizes to unseen images while remaining transparent and explainable.

---

### Key Idea
The project demonstrates how reasoning-based models can serve as symbolic optimizers — writing, testing, and improving code to align quantitative metrics with qualitative human perception.  
It highlights a broader idea: *AI shouldn’t just mirror data; it should learn to see and judge with human-like discernment and taste.*

---

### Repository Contents
- `Aesthetic_Reward_Function.ipynb` — main notebook with exploration, attribute analysis, and reward design  
- `train_scores.csv` and `test_scores.csv` — human-annotated scores and abstract visual attributes assigned to images 

