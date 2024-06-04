I trained a neural network on 32k names using bigrams to get the probabilities of characters following one another. In this model, which is made in PyTorch, P(cᵢ₊₁ | cᵢ)
is learned for each character pair and it creates a stochastic matrix that embodies the language’s morphological structure. Additionally, this could be turned into something 
as modern as a Transformer language model such as GPT.

Key steps:

Bigram extraction & frequency mapping

PyTorch matrix for transition probabilities

Neural net training via cross-entropy & backpropagation

Sampling with torch.multinomial

It encompasses modeling of sampling and training of models including evaluation of loss (e.g., negative log likelihood for classification).

A neural network was implemented and then prediction model optimized through gradient descent resulting in reduction of loss function by backpropagation.

Result: A model that generates linguistically plausible names indicating that local character dependencies heavily influence global word structure.
This approach goes beyond names; it can apply to any area governed by sequential patterns such as code prediction, melody generation or even DNA sequence modeling.
