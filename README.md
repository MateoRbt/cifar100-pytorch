# CIFAR-100 Benchmarking with ResNet-18 and ShuffleNet v2

## Objective
This project compares two popular CNN architectures 
— ResNet-18 and ShuffleNet v2 
— trained on CIFAR-100 
with varying amounts of training data (70%, 60%, 50%). The goal is to evaluate their performance and robustness under limited data scenarios.

## Training Setup
Dataset: CIFAR-100

1) Loss Function: CrossEntropyLoss

2) Optimizer: SGD (momentum = 0.9, weight decay = 5e-4)

3) Batch size: 256

4) Learning rate: 0.01

5) Epochs:

    Α) ResNet-18: 30

    Β) ShuffleNet v2: 100
## Results Summary
| Data Used | Model         | Accuracy | Precision | Recall | F1-score |
| --------- | ------------- | -------- | --------- | ------ | -------- |
| **70%**   | ResNet-18     | 0.8024   | 0.8044    | 0.8024 | 0.8022   |
|           | ShuffleNet v2 | 0.7576   | 0.7597    | 0.7576 | 0.7574   |
| **60%**   | ResNet-18     | 0.7981   | 0.8013    | 0.7981 | 0.7985   |
|           | ShuffleNet v2 | 0.7417   | 0.7442    | 0.7417 | 0.7418   |
| **50%**   | ResNet-18     | 0.7821   | 0.7849    | 0.7821 | 0.7824   |
|           | ShuffleNet v2 | 0.7212   | 0.7233    | 0.7212 | 0.7206   |
