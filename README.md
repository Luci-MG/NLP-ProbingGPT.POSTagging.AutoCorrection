# NLP Project

This repository contains three sub-projects focused on Natural Language Processing (NLP): ProbingGPT, Postagging, and Autocorrection. Each sub-project addresses different aspects of NLP, utilizing various techniques and algorithms.

## Table of Contents
1. [ProbingGPT](#probinggpt)
    - [Overview](#overview)
    - [How to Run](#how-to-run)
    - [Results and Evaluation](#probinggpt-results-and-evaluation)
2. [Postagging](#postagging)
    - [Overview](#overview-1)
    - [How to Run](#how-to-run-1)
    - [Results and Evaluation](#postagging-results-and-evaluation)
3. [Autocorrection](#autocorrection)
    - [Overview](#overview-2)
    - [How to Run](#how-to-run-2)
    - [Results and Evaluation](#autocorrection-results-and-evaluation)
4. [License](#license)
5. [Acknowledgements](#acknowledgements)
6. [Contributing](#contributing)

## ProbingGPT

### Overview
The ProbingGPT sub-project, inspired by the methodology outlined in the [paper](https://arxiv.org/abs/1610.01644), utilizes the [Baukit](https://github.com/davidbau/baukit) library to probe the [GPT-2](https://huggingface.co/docs/transformers/v4.35.0/en/model_doc/gpt2#transformers.GPT2LMHeadModel) small model downloaded from Hugging Face. Focused on layers h.0.mlp, h.3.mlp, h.9.mlp, and h.9.attn, the project employs the [SNLI](https://nlp.stanford.edu/pubs/snli_paper.pdf) corpus to generate text. Hidden states from these layers are captured through Baukit probing, and linear classifiers are trained on them. The evaluation aims to assess the model's understanding of contradictions, neutral and entailments and how well the model learns at each layer, all executed in [Google Colab](https://colab.research.google.com/) for seamless collaboration and execution.

### How to Run & ProbingGPT Results and Evaluation

Import the [Jupyter file](ProbingGPT/NLPProbingGPT.ipynb) into Google Colab and follow the provided instructions. All the results and evaluations are present in the same file.
