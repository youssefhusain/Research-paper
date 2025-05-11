#  Comparison of Models in the Paper: Tanh vs GRU vs LSTM

##  Paper: Empirical Evaluation of Gated Recurrent Neural Networks on Sequence Modeling
**Authors:** Junyoung Chung, Caglar Gulcehre, KyungHyun Cho, Yoshua Bengio  
**Link:** [arXiv:1412.3555](https://arxiv.org/pdf/1412.3555)

---

##  Model Comparison Table

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
  ![DataCamp](img/p1(1).png)
##  Key Insights from the Paper

###  1. Gated Units Perform Better
- Both **GRU** and **LSTM** significantly outperform the traditional **tanh** RNN.
- They are especially better at modeling long-range dependencies in sequence tasks.

  ###  2. Task Results
- **On polyphonic music modeling and speech signal modeling:**
  - **GRU and LSTM** clearly outperform tanh.
  - In some cases, **GRU performed even better than LSTM** despite being simpler.
  - ![DataCamp](img/p1(2).png)

