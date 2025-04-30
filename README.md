# Semi-Supervised Learning for Handwritten Digit Recognition

This project demonstrates the use case of semi-supervised learning techniques on handwritten digit recognition using the MNIST dataset. By combining a convolutional neural network (CNN) with clustering, consistency regularization, and entropy minimization, the model can achieve a high classification accurary with a small set of labeled data and a larger set of unlabeled data.

## Abstract

The goal of this project is to improve classification accuracy when only limited labeled data is available. In our experiments, the model used from 10% to less than 0.1% of the data as labeled data, while the remaining data was treated as unlabeled. The model includes:

- **Clustering Loss**: Encourages feature representations of unlabeled data to be close to the centroids computed from labeled data.

- **Consistency Loss**: Ensures the model produces similar outputs for an image and its augmented version.

- **Entropy Minimization**: Pushes the model toward making confident predictions on unlabeled data.

The results show that despite labeling 10% of the dataset, our method reaches 98% accuracy.