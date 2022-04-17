# Recurrent Neural Networks (RNN)

## Perplexity (Evaluation of the language model)

The perplexity shows how much varied the predicted distribution for the next word is. This ensures that sequences of different length are comparable.

- In the best case scenario, the model always perfectly estimates the probability of the label token as 1. In this case the perplexity of the model is 1.

- In the worst case scenario, the model always predicts the probability of the label token as 0. In this situation, the perplexity is positive infinity.

- At the baseline, the model predicts a uniform distribution over all the available tokens of the vocabulary. In this case, the perplexity equals the number of unique tokens of the vocabulary. In fact, if we were to store the sequence without any compression, this would be the best we could do to encode it. Hence, this provides a nontrivial upper bound that any useful model must beat.

## Hidden State

It is noteworthy that hidden layers and hidden states refer to two very different concepts. 
- Hidden layers are layers that are hidden from view on the path from input to output. 
- Hidden states are technically speaking inputs to whatever we do at a given step, and they can only be computed by looking at data at previous time steps.


## Gradient clipping

Gradient clipping provides a quick fix to the gradient exploding. It ensures that the model does not diverge even when gradients blow up at some point during the training process.

## Gated Recurrent Units (GRU)

- Reset gates help capture short-term dependencies in sequences.
- Update gates help capture long-term dependencies in sequences.

## Long Short-term Memory (LSTM)

This design is introduced to alleviate the vanishing gradient problem and to better capture long range dependencies within sequences.

LSTMs have three types of gates: input gates, forget gates, and output gates that control the flow of information.

### GRU vs LSTM
-  The GRU is a slightly more streamlined variant that often offers comparable performance and is significantly faster to compute
-  Training LSTMs and other sequence models (such as GRUs) are quite costly due to the long range dependency of the sequence. (addressed by transformers)
