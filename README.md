# BNeCR V1.0

BNeCR is a diagnostic benchmark designed to evaluate the ability of large language models (LLMs) to reason about *newly introduced concepts* that are not present in their pre-training data. Unlike conventional benchmarks that primarily test factual recall or reasoning over known concepts, BNeCR focuses on controlled conceptual novelty and reasoning under limited information.

This repository provides the full dataset, data format specifications, and example usage to support reproducibility and future research.

---

## 📌 Motivation

Recent large language models have demonstrated impressive performance on a wide range of benchmarks. However, high accuracy often arises from memorization, pattern matching, or shortcut strategies rather than genuine reasoning. Evaluating whether LLMs can *understand and reason about previously unseen concepts* remains an open challenge.

BNeCR is designed to address this gap by:
- Introducing **synthetically coined concepts** absent from existing corpora,
- Embedding concepts in **controlled contextual or analogical settings**, and
- Employing **semantically plausible distractors** to reduce superficial elimination strategies.

---

## 🧠 Task Overview

Each instance in BNeCR presents:
- A **novel concept name**,
- A **contextual description** and/or **analogical reference**,
- A **multiple-choice question** with one correct answer and several distractors.

Models are required to infer the meaning or properties of the new concept based solely on the provided information.

### Reasoning Conditions

The dataset is organized into three reasoning conditions:
- **CA (Context + Analogy)**: Both contextual description and analogical support are provided.
- **OC (Only Context)**: Only contextual information is available.
- **NC (No Context)**: No explicit supporting information is given.

This structure enables controlled analysis of how different forms of reasoning support affect model behavior.

---


