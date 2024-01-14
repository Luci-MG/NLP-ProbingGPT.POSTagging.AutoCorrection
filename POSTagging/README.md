# Part-of-Speech Tagging Results

## Hidden Markov Models (HMM)

### Token Counts

😱

- English (~40000)
- Japanese (~17000)
- Bulgarian (~13000)

#### Emission and Transition Probabilities

| Model   |  English (~40000)   | Japanese (~17000)    | Bulgarian (~13000)|
|---------|--------|--------|--------|--------|--------|--------|
|         | ERW | ERS | ERW| ERS| ERW| ERS|
|         |        |        |        |        |        |        |
| Bigram  | 0.054  | 0.655  | 0.062  | 0.136  | 0.115  | 0.751  |
| Trigram | 0.049  | 0.613  | 0.063  | 0.133  | 0.110  | 0.721  |

## Recurrent Neural Networks (RNNs)

### Token Counts

😱

- English (~40000)
- Japanese (~17000)
- Bulgarian (~13000)

#### Accuracy Scores

| Model      | ERW     | ERS     | ERW     | ERS     | ERW     | ERS     |
|------------|---------|---------|---------|---------|---------|---------|
|            | Vanilla | Vanilla | Vanilla | LSTM    | LSTM    | LSTM    |
|            | RNN     | RNN     | RNN     |         |         |         |
|            |         |         |         |         |         |         |
| English    | 0.295   | 0.758   | 0.105   | 0.155   | 0.572   | 0.809   |
| Japanese   | 0.291   | 0.748   | 0.117   | 0.191   | 0.575   | 0.821   |
| Bulgarian  | 0.283   | 0.714   | 0.103   | 0.135   | 0.558   | 0.804   |

