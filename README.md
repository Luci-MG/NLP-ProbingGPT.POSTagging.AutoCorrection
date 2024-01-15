# NLP-ProbingGPT2/POS-Tagging/AutoCorrection

This repository contains three sub-projects focused on Natural Language Processing (NLP): ProbingGPT, Postagging, and Autocorrection. Each sub-project addresses different aspects of NLP, utilizing various techniques and algorithms.

## Table of Contents
1. [ProbingGPT](#probinggpt)
    - [Overview](#overview)
    - [How to Run Results and Evaluation](#how-to-run-results-and-evaluation)
2. [Postagging](#postagging)
    - [Overview](#overview-1)
    - [How to Run and Evaluation](#how-to-run-and-evaluation)
    - [Results and Evaluation](#postagging-results-and-evaluation)
3. [Autocorrection](#autocorrection)
    - [Overview](#overview-2)
    - [How to Run and Perfomance check](#how-to-run-and-perfomance-check)
4. [Contributing](#contributing)

## ProbingGPT

### Overview
The ProbingGPT project, inspired by the methodology outlined in the [paper](https://arxiv.org/abs/1610.01644), utilizes the [Baukit](https://github.com/davidbau/baukit) library to probe the [GPT-2](https://huggingface.co/docs/transformers/v4.35.0/en/model_doc/gpt2#transformers.GPT2LMHeadModel) small model downloaded from Hugging Face. Focused on layers h.0.mlp, h.3.mlp, h.9.mlp, and h.9.attn, the project employs the [SNLI](https://nlp.stanford.edu/pubs/snli_paper.pdf) corpus to generate text. Hidden states from these layers are captured through Baukit probing, and linear classifiers are trained on them. The evaluation aims to assess the model's understanding of contradictions, neutral and entailments and how well the model learns at each layer, all executed in [Google Colab](https://colab.research.google.com/) for seamless collaboration and execution.

### How to Run Results and Evaluation
Import the [Jupyter file](ProbingGPT/NLPProbingGPT.ipynb) into Google Colab and follow the provided instructions. All the results and evaluations are present in the same file.

## Postagging

### Overview
The Postagging sub-project explores part-of-speech tagging using Hidden Markov Models (HMM) with bigram and trigram implementations. The study covers three languages: English, Japanese, and Bulgarian. Additionally, the performance of Vanilla RNN, LSTM, and Bidirectional LSTM models is compared for part-of-speech tagging.

### How to Run and Evaluation
1. For HMM with Viterbi Algo
```python
python3 train_hmm.py data/ptb.2-21.tgs data/ptb.2-21.txt > my.hmm # for training
python3 viterbi.py my.hmm < data/ptb.22.txt > my.out # for viterbi
python3 tag_acc.py data/ptb.22.tgs my.out # for eval
```
2. For VRNN, LSTM, BIDLSTM
```python
python3 vrnn_lstm_bidlstm.py data/ptb.2-21.tgs data/ptb.2-21.txt data/ptb.22.tgs data/ptb.22.txt 22_1.out # for training and eval
```

### Postagging Results and Evaluation
Detailed Evaluated results are provided in [results/README.md](Postagging/README.md) file.

## Autocorrection

### Overview
Autocorrection focuses on evaluating different spell correction methods, including bigram, unigram, trigram, smoothed bigram, bigram with backoff, smoothed unigram, and trigram with backoff. The project uses an edit model for autocorrection and compares the performance of each method based on evaluation metrics.

### How to Run and Perfomance check
```python
python3 EditModel.py # for sanity check your edit model
python3 SpellCorrect.py # for performance of all the language models
```

## Contributing
If you would like to contribute or report issues, please mail to **Email:** mg6.dev@gmail.com
