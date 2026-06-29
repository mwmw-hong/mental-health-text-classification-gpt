# Mental Health Text Classification with GPT-Based Models

This repository contains a university research project evaluating GPT-based approaches for classifying mental-health-related online texts. The project compares prompt engineering, DSPy, retrieval-augmented generation (RAG), and traditional machine learning baselines.

The full paper is available in [`paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf`](paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf).

## Project Overview

The goal of this project was to evaluate how effectively GPT-based models can classify depression severity in online text. The work explores both LLM-based workflows and classical machine learning methods, with an emphasis on comparing model behavior across different approaches.

## Methods

- Exploratory data analysis and preprocessing
- Prompt engineering with GPT models
- DSPy-based prompting workflows
- Retrieval-augmented generation using LangChain and vector search
- Naive Bayes and Logistic Regression baselines

## Repository Structure

```text
.
|-- notebooks/
|   |-- Script-1-Preprocessing-EDA.ipynb
|   |-- Script-2-Prompt-Engineering.ipynb
|   |-- Script-2.1-Prompt-Engineering.ipynb
|   |-- Script-2.2-Prompt-Engineering.ipynb
|   |-- Script-3-DSPy.ipynb
|   |-- Script-4-RAG.ipynb
|   `-- Script-5-NB_LR.ipynb
|-- paper/
|   `-- Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf
`-- README.md
```

## Notes on Data and Reproducibility

The notebooks reference local dataset paths used during the original research. The dataset files are not included in this repository, so paths may need to be adjusted before rerunning the notebooks.

Notebook outputs have been cleared for privacy and readability. This keeps the code and methodology visible while avoiding publication of raw mental-health text excerpts, local machine paths, or generated logs.

## Tools and Libraries

- Python
- Jupyter Notebook
- pandas
- scikit-learn
- OpenAI API
- DSPy
- LangChain
- Chroma

## Paper

For full methodology, evaluation details, and results, see the included PDF paper:

[`Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf`](paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf)
