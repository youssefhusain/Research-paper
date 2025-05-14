#  Summary of "Attention is All You Need"
![](img/sat1.png)
In 2017, the deep learning landscape shifted dramatically with the introduction of the **Transformer** model. Unlike previous methods that depended on recurrent or convolutional layers, this architecture proposed a bold idea: _remove recurrence altogether and use attention as the sole mechanism for modeling dependencies_.

---

## Why Move Beyond RNNs?

Traditional models like **RNNs** and **LSTMs** were once the standard for tasks such as language translation and text generation. However, they had several drawbacks:
- **Sequential computation** slowed down training.
- **Long-range dependencies** were hard to capture.
- **Parallelization** was limited due to step-by-step processing.

The Transformer addressed all of these by processing the entire sequence at once, using **self-attention**.

---

## Key Mechanisms That Power the Transformer

Instead of recurrence, the Transformer uses:

- **Self-Attention Layers**: Each element in the input sequence pays "attention" to every other element, enabling better context understanding.
  
- **Multi-Head Attention**: Multiple attention layers run in parallel, allowing the model to learn different types of relationships between words.
  
- **Feed-Forward Networks**: Applied after attention to transform the output further.

- **Positional Encodings**: Since the model doesn’t inherently track order, positional info is added to input embeddings using sine and cosine patterns.

---
##  Key Concepts

- **Self-Attention**: Allows the model to relate different positions of a sequence to each other in a single step.
- **Multi-Head Attention**: Enables the model to attend to information from different representation subspaces at different positions.
- **Positional Encoding**: Injects sequence order information into input embeddings.
- **Encoder-Decoder Architecture**:
  - **Encoder**: A stack of layers with self-attention + feed-forward networks.
  - **Decoder**: Similar to encoder but includes encoder-decoder attention.
- **Performance**: Achieved state-of-the-art results on English-German and English-French translation tasks with faster training compared to RNN-based models.

---

![](img/sat2.png)
