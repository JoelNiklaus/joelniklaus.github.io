---
title: "Data Augmentation for Legal NLP"
article: "#"
print: "#"
dataset: "#"
code: "#"
models: "#"
---

### Introduction

Legal Judgment Prediction is an NLP task that automatically predicts the judgment outcome based on the facts of a case. In our dataset, we only have around 4K Italian decisions but more than 31K French decisions and almost 50K German decisions. As can be expected, the performance on the Italian dataset is much worse compared to the French and German dataset. In this project, you will experiment with data augmentation techniques \[2\] such as back-translation or machine-translating decisions from high-resource (many data points) languages (German and French in our case) to low-resource (few data points) languages (Italian in our case).

