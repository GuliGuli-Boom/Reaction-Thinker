
# Towards Knowledge‑and‑Data‑Driven Organic Reaction Prediction: RAG‑Enhanced and Reasoning‑Powered Hybrid System with LLMs

<p align="center">
  <img src="./assets/architecture.png" width="85%">
</p>

<p align="center">
  🔬 ICLR 2026 | 🧪 LLM for Chemistry | ⚡ RAG + Reasoning
</p>

---

## 📌 Highlights

- 🧠 **Hybrid LLM System**: Combines Retrieval-Augmented Generation (RAG) and reasoning-based models  
- 🔍 **Knowledge Injection**: Similar reaction retrieval improves factual grounding  
- 🔗 **Chain-of-Thought Reasoning**: Explicit reaction mechanism modeling  
- ⚡ **RL Optimization (GRPO)**: Enhances reasoning accuracy  
- 🏆 **SOTA Performance** on Open Reaction Dataset (ORD)

---

## 📖 Abstract

We propose **Reaction-Thinker**, a hybrid framework that integrates:

- Data-driven learning (SFT)
- Knowledge-driven retrieval (RAG)
- Reasoning optimization (RL with GRPO)

to improve both **accuracy** and **interpretability** in organic reaction prediction.

---

## 🏗️ System Architecture

<p align="center">
  <img src="./assets/architecture.png" width="90%">
</p>

### 🔧 Components

1. **Reaction Type Classifier**
   - Input: SMILES
   - Output: reaction type + embedding

2. **Retrieval Module**
   - L2 distance over learned embeddings
   - Builds type-specific retrieval database

3. **RAG-based Predictor**
   - Injects retrieved cases into prompt

4. **Reasoning-based Predictor**
   - CoT-based deduction when no similar cases exist

---

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourname/reaction-thinker.git
cd reaction-thinker
