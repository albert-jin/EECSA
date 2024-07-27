# EECSA: Emotion-Enriched Contextual Sentiment Analysis through LLM Prompting
Code Implementation about paper: "Enhancing Textual Sentiment Analysis through Emotion-Enriched Contextual Integration and Self-Adaptive Prompting Optimization"

## Overview

Textual Sentiment Analysis (TSA) is a crucial task in natural language processing (NLP) that identifies sentiment towards specific entities or aspect terms within a text. Traditional deep learning-based TSA methods often face challenges such as large domain-specific training data requirements and poor domain transferability. To address these issues, we propose the EECSA framework.

EECSA leverages unique emotion-enriched contextual constraints, backgrounds, and analogical reasoning to address LLM hallucinations and enhance sentiment prediction accuracy. The framework integrates various in-context augmentation strategies, including emotion-oriented backgrounds, constraints, and analogical reasoning, further improving initial LLM instructions through adaptive iterative optimization using a random search bootstrap algorithm.

[![](/results/EECSA.png "Architecture of EECSA")][Architecture of EECSA]


## Key Features

- **Emotion-Enriched Contextual Constraints:** Constructs variant queries hypothesizing different polarities for aspect terms within a sentence, ensuring consistency and accuracy through a secondary evaluation mechanism.
- **Emotion-Enriched Contextual Backgrounds:** Integrates aspect term background information into sentiment identification, enhancing the precision of sentiment analysis by leveraging LLM's ability to provide context-aware information.
- **Emotion-Enriched Contextual Analogies:** Utilizes analogical reasoning to generate emotionally and contextually relevant examples, guiding the LLM in solving sentiment analysis tasks more effectively.
- **Self-Adaptive Bootstrap Instructions Optimization:** Enhances LLM predictions by iteratively refining prompts and examples, maximizing the benefits of LLM prompting.

## Performance

Extensive zero/few-shot experiments with GPT-3.5-turbo across six public datasets validate the effectiveness and robustness of EECSA, even surpassing GPT-4.0 in certain scenarios, the most advanced large language model in the world.

[![](/results/zero-shot.png "Zero Shot Performance of EECSA")][Zero Shot Performance of EECSA]

## Datasets

- **SemEval-2014:** Includes benchmarks for both the restaurant and laptop domains.
- **SemEval-2015:** Focuses on the restaurant domain.
- **SemEval-2016:** Covers the restaurant domain with diverse datasets.
- **Twitter:** Annotated tweets from the Twitter platform.
- **ACLShortData:** Social tweets annotated via Amazon Mechanical Turk.

## Comparison with Baselines

The EECSA framework demonstrates significant improvements over traditional and LLM-based baselines in zero-shot and few-shot settings. It systematically optimizes LLM instructions through emotion-enriched contexts and self-adaptive bootstrap instructions optimization, achieving higher accuracy in sentiment analysis tasks.


## Getting Started

To run the EECSA framework, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/albert-jin/EECSA.git
   ```

2. Using these files at Google Colab or Python Jupyter Notebook.
   ```bash
   Run XXX.ipynb
   ```
   

