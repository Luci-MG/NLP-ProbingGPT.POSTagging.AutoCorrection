# Part-of-Speech Tagging Results

### Evaluations
- ERW - Error rate by word
- ERS - Error rate by sentence

### Token Counts
- English (~40000) (ENG)
- Japanese (~17000) (JP)
- Bulgarian (~13000) (BG)

## Hidden Markov Models (HMM)

#### Emission and Transition Probabilities
| Model      | ENG     | ENG     | JP     | JP     | BG     | BG     |
|------------|---------|---------|---------|---------|---------|---------|
|            | ERW | ERS | ERW | ERS    | ERW    | ERS    |
| Bigram  | 0.054  | 0.655  | 0.062  | 0.136  | 0.115  | 0.751  |
| Trigram | 0.049  | 0.613  | 0.063  | 0.133  | 0.110  | 0.721  |

## Recurrent Neural Networks (RNNs)

#### Emission and Transition Probabilities

| Model      | ENG     | ENG     | JP     | JP     | BG     | BG     |
|------------|---------|---------|---------|---------|---------|---------|
|            | ERW | ERS | ERW | ERS    | ERW    | ERS    |
| Vanilla RNN    | 0.295   | 0.758   | 0.105   | 0.155   | 0.572   | 0.809   |
| LSTM   | 0.291   | 0.748   | 0.117   | 0.191   | 0.575   | 0.821   |
| BIDLSTM  | 0.283   | 0.714   | 0.103   | 0.135   | 0.558   | 0.804   |

## POS-Tagged data analysis plot - Learning Curve if Bigram HMM

![Analysis Plot](Figure_4_normalizederserwplot.png)


