#  Comparison of Models in the Paper: Tanh vs GRU vs LSTM

##  Paper: Empirical Evaluation of Gated Recurrent Neural Networks on Sequence Modeling
**Authors:** Junyoung Chung, Caglar Gulcehre, KyungHyun Cho, Yoshua Bengio  
**Link:** [arXiv:1412.3555](https://arxiv.org/pdf/1412.3555)

---

## 📊 Model Comparison Table

| Feature / Model                          | Tanh Model                         | GRU Model                                       | LSTM Model                                      |
|------------------------------------------|------------------------------------|-------------------------------------------------|------------------------------------------------|
| **Type**                                 | Basic RNN                          | Gated Recurrent Unit (GRU)                      | Long Short-Term Memory (LSTM)                   |
| **Number of Gates**                      | None                               | 2 (Update, Reset)                               | 3 (Input, Forget, Output)                       |
| **Long-term Dependency Handling**        | Poor                               | Strong                                          | Very Strong                                     |
| **Computational Complexity**             | Low                                | Medium                                          | High                                            |
| **Internal Memory (Cell State)**         | no                                 | yes                                             | yes                                             |
| **Training Stability**                   | Less stable                        | Stable                                          | Stable                                          |
| **Performance on Sequence Tasks**        | Worst                              | Comparable to or better than LSTM               | Slightly better than GRU                        |

---
