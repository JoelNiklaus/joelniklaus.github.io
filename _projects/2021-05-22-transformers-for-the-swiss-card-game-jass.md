---
title: "Transformers for the Swiss Card Game Jass"
---

### Introduction

Despite the recent successful application of Artificial Intelligence (AI) to games, the performance of cooperative agents in imperfect information games is still far from surpassing humans. Cooperating with teammates whose play-styles are not previously known poses additional challenges to current state-of-the-art algorithms. In the Swiss card game Jass, coordination between the two opposing teams is crucial for winning. Since verbal communication is forbidden, the only way to transmit information within the team is through a player’s play-style. This makes the game a particularly suitable candidate subject to continue the research on AI in cooperation games with hidden information. The best computer programs can compete with strong amateur players in the Schieber variant of the popular Swiss card game Jass \[1\]. Convolutional neural networks (CNN) are on par with Monte Carlo Tree Search (MCTS) in Schieber.

### Research Questions

So far, the transformer architecture has not been applied to Schieber yet.

RQ1: Can the transformer architecture improve on the state-of-the-art in Schieber?

RQ2: To what extent can the transformer architecture learn cooperation strategies with the partner?

### Steps

1.  Understand the transformer architecture \[2\]
2.  Integrate the transformer into the existing codebase
3.  Train the transformer
4.  Experiment with different hyperparameters
5.  Evaluate the results

### Activities

⬤⬤◯◯◯ Programming

⬤⬤⬤⬤◯ Experimentation

⬤◯◯◯◯ Literature

### Prerequisites

Good programming skills (preferably in Python)

Experience with Machine Learning and Neural Networks

### Contact

[Joel Niklaus](https://www.digitale-nachhaltigkeit.unibe.ch/about_us/persons/niklaus_joel/index_eng.html)

### References

\[1\] Niklaus, J., Alberti, M., Ingold, R., Stolze, M., & Koller, T. (2020). Challenging Human Supremacy: Evaluating Monte Carlo Tree Search and Deep Learning for the Trick Taking Card Game Jass. _ICAISC_.

\[2\] Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. _ArXiv, abs/1706.03762_.