# Neural_Network_Charity_Analysis
In this project, I attempt to identify charitable projects which should and should not receive donations from a hypothetical donor using neural networks. 

Preprocessing steps include binning and encoding of categorical data and feature selection and made use of pandas and sklearn libraries. The model was constructed using Python's tensorflow and keras libraries. 

The naive (first-attempt) model used 2 hidden layers, with 8 and 5 nodes, respectively. It received the following performance report, where the loss metric is binary crossentropy.

```
268/268 - 1s - loss: 0.6950 - accuracy: 0.6588
Loss: 0.6949737668037415, Accuracy: 0.6587755084037781
```

Three attempts were made at optimizing the model. The first (Optimization1) removed one more feature from the model, which resulted in a higher accuracy and higher loss than the naive model.

```
268/268 - 1s - loss: 0.8056 - accuracy: 0.7018
Loss: 0.8056194186210632, Accuracy: 0.7018075585365295
```

Two additional optimization attempts were made of Optimization1.

Optimization2 added an additional hidden layer with three nodes to the model. This resulted in lower loss and accuracy.

```
268/268 - 1s - loss: 0.7155 - accuracy: 0.5332
Loss: 0.7155246138572693, Accuracy: 0.5331778526306152
```

Optimization3 used the same number of hidden layers as Optimization1, but changed the hidden layer activation function from relu to tanh. This also resulted in lower loss and lower accuracy.

```
268/268 - 1s - loss: 0.6808 - accuracy: 0.5645
Loss: 0.6808474659919739, Accuracy: 0.5645480751991272
```
