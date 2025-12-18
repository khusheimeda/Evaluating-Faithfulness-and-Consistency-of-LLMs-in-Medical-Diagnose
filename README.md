# Evaluating Faithfulness and Consistency of LLMs in Medical Diagnosis

This repository contains the code and experimental framework for a final project (CS685) evaluating the reliability of Large Language Models (LLMs) when applied to medical diagnostic tasks.

The project focuses on two critical dimensions of trustworthiness: **Faithfulness** (reasoning grounded in input) and **Consistency** (robustness across semantic variations).

## Repository Structure

The codebase is organized into five main directories, each targeting a specific evaluation metric:

### 1. [Input Attribution](./Input%20Attribution)
Focuses on faithfulness by analyzing feature attribution. This module determines which parts of the medical history or patient description the LLM attends to when making a diagnosis.
* **Goal:** Verify if the model relies on medically relevant symptoms vs. spurious correlations.

### 2. [Paraphrase Consistency](./Paraphrase_consistency)
Evaluates the model's robustness to surface-level changes in the input text.
* **Goal:** Ensure that rephrasing a patient's symptoms (without changing the semantic meaning) does not result in a contradictory diagnosis.

### 3. [Causal Direction Consistency](./causal%20direction%20consistency)
Tests the model's understanding of causal relationships in medical reasoning.
* **Goal:** Check if the model consistently distinguishes between causes (e.g., a disease) and effects (e.g., symptoms) and maintains logical consistency when causal directions are manipulated.

### 4. [False Premise](./false%20premise)
Investigates the model's behavior when presented with hallucinated or incorrect medical premises.
* **Goal:** Assess if the model accepts false premises as true or corrects them/expresses uncertainty.

### 5. Irrelevant Information Overload and Leading Questions
Investigates the faithfulness of scenarios where input has irrelevant information and leading questions which are erraneous.

## 🚀 Getting Started

### Prerequisites
* Python 3.8+
* Jupyter Notebook
* Required libraries: `transformers`, `torch`, `scikit-learn`, `pandas`, `numpy`

### Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/himaj264/NLP-Evaluating-Faithfulness-and-Consistency-of-LLMs-in-Medical-Diagnose.git](https://github.com/himaj264/NLP-Evaluating-Faithfulness-and-Consistency-of-LLMs-in-Medical-Diagnose.git)
   cd NLP-Evaluating-Faithfulness-and-Consistency-of-LLMs-in-Medical-Diagnose
