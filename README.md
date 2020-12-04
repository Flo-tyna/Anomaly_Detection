# Anomaly_Detection
Anomaly Detection using Deep Learning (Autoencoders in Tensorflow)
The idea is quite simple:
* The bottleneck architecture of the autoencoder in neural networks, forces the model to learn a condensed representation in order to reproduce the original input.
* By feeding the encoder onlynon-fraudulent transaction data, the encoder model learns the characteristics of these non-fraudulent transactions and can identify it with high fidelity.
* Now that the model can detect non-fraudulent transactions, the remainder transactions fall into the fraudulent category.Thus the auto-encoder will have trouble reproducing it with its learned weights, and the subsequent reconstruction loss will be high.
* Anything above a specific loss (treshold) will be flagged as anomalous and thus labeled as fraud.
