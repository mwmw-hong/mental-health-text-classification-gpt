# Mental Health Text Classification with GPT-Based Models

This repository contains a university research project evaluating GPT-based approaches for classifying depression severity from Reddit-based mental-health text. The project compares GPT-3.5 Turbo, GPT-4o, DSPy, retrieval-augmented generation (RAG), and traditional machine learning baselines.

The full research paper is available in [`paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf`](paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf).

## Key Results

The project compared LLM-based approaches and traditional machine learning models for multiclass depression severity classification.

| Method | Macro F1 | RMSE | Notes |
|---|---:|---:|---|
| GPT-3.5 Turbo baseline | 0.21 | 1.44 | Initial GPT-3.5 baseline |
| GPT-3.5 Turbo few-shot | 0.33 | 1.19 | Improved with examples |
| GPT-3.5 Turbo DSPy | 0.39 | 1.11 | Best GPT-based method |
| Logistic Regression | 0.41 | 1.36 | Strong traditional baseline |
| Multinomial Naive Bayes | 0.31 | 1.80 | Traditional baseline |

Key findings:

- DSPy achieved the largest improvement, increasing macro F1 by 46.2% compared with the GPT-3.5 baseline while reducing RMSE by 29.7%.
- Few-shot prompting improved macro F1 by 26.5% and reduced RMSE by 17.2% over the baseline.
- Manual prompt engineering with enhanced zero-shot prompting improved macro F1 by approximately 10%.
- RAG produced mixed results, slightly lowering classification performance but reducing prediction error in some configurations.
- Logistic Regression remained highly competitive, achieving a macro F1 score of 0.41 compared with 0.39 for the best DSPy model.

## My Contribution

My primary responsibilities included:

- Developed the DSPy implementation for automated prompt optimization using the MIPROv2 optimizer.
- Implemented the Logistic Regression benchmark classifier using TF-IDF features.
- Implemented the Multinomial Naive Bayes benchmark classifier.
- Conducted comparative experiments between traditional machine learning models and GPT-based approaches.
- Explored and evaluated emerging LLM technologies and prompt optimization techniques.
- Assisted in performance evaluation, result interpretation, and analysis of model effectiveness.

## Skills Demonstrated

Machine learning:

- Text classification
- Logistic Regression
- Multinomial Naive Bayes
- TF-IDF feature engineering
- Model evaluation and benchmarking

Natural language processing:

- Prompt engineering
- Few-shot learning
- Chain-of-Thought prompting
- Retrieval-Augmented Generation (RAG)
- Automated prompt optimization with DSPy

Large language models:

- OpenAI API
- GPT-3.5 Turbo
- GPT-4o
- DSPy framework

Data science:

- Experimental design
- Performance evaluation
- Hyperparameter experimentation
- Error analysis
- Imbalanced dataset handling

Python ecosystem:

- pandas
- NumPy
- scikit-learn
- LangChain
- ChromaDB
- Jupyter Notebooks

## Methods

- Exploratory data analysis and preprocessing
- Manual prompt engineering with zero-shot, few-shot, and Chain-of-Thought prompting
- DSPy-based automated prompt optimization
- Retrieval-Augmented Generation using LangChain and ChromaDB
- Traditional machine learning baselines with Naive Bayes and Logistic Regression
- Evaluation using macro F1, accuracy, MAE, and RMSE

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
|-- .gitignore
`-- README.md
```

## Notebook Execution Order

Run the notebooks in the following order:

| Step | Notebook | Purpose |
|---:|---|---|
| 1 | `Script-1-Preprocessing-EDA.ipynb` | Data loading, preprocessing, and exploratory data analysis |
| 2 | `Script-2-Prompt-Engineering.ipynb`, `Script-2.1-Prompt-Engineering.ipynb`, `Script-2.2-Prompt-Engineering.ipynb` | Manual prompt engineering experiments with zero-shot, few-shot, and Chain-of-Thought prompting |
| 3 | `Script-3-DSPy.ipynb` | Automated prompt optimization using DSPy |
| 4 | `Script-4-RAG.ipynb` | Retrieval-Augmented Generation experiments using LangChain and ChromaDB |
| 5 | `Script-5-NB_LR.ipynb` | Traditional machine learning baselines with Naive Bayes and Logistic Regression |

Running the LLM notebooks requires an OpenAI API key and may incur API costs. The DSPy and RAG notebooks also require the appropriate API credentials and dependencies.

## Notes on Data and Reproducibility

The original research used the Dreaddit and DepSeverity datasets. Dataset files are not included in this repository, so local dataset paths may need to be adjusted before rerunning the notebooks.

Notebook outputs have been cleared for privacy and readability. This keeps the code and methodology visible while avoiding publication of raw mental-health text excerpts, local machine paths, or generated logs.

## Ethical Considerations

This project investigates depression severity classification and is intended solely as a research project, not as a clinical diagnostic system.

Key ethical considerations:

- The models should not be used for medical diagnosis or treatment decisions without qualified healthcare professionals.
- Reddit posts may not accurately reflect an individual's mental health, and language alone cannot reliably diagnose depression.
- Large Language Models may inherit biases from their training data, potentially affecting predictions across demographic groups.
- The dataset consists of publicly available Reddit posts that were previously collected and annotated for research purposes.
- Any deployment of similar systems should include human oversight, transparency regarding model limitations, and careful consideration of privacy and fairness.

## Paper

For full methodology, evaluation details, and results, see the included PDF paper:

[`Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf`](paper/Evaluating_GPT_Based_Models_for_Classifying_Mental_Health_in_Online_Texts.pdf)
