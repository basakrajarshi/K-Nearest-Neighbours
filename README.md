# K-Nearest-Neighbours
Implementation of the KNN algorithm on the mnist.pklz dataset to classify images. Here we take an image of a handwritten digit and predict which digit it corresponds to.

The following functions were built for the problem:

(i) the label_counts function which returns a dictionary of frequencies corresponding to each label in the training set.

(ii) the majority function whichc returns the label that appears most frequently in the  KK -nearest neighbors of the query point. In the case that the maximum frequency occurs for two or more labels, it returns the one that appears most frequently in the entire training set. In the case that there is still a tie, it breaks the tie in any way that you choose.

(iii) the classify function which finds the indices of the  K  closest training examples to the query point and then calls the majority function to return the predicted label. Almost all of the heavy lifting here is done by the BallTree object from sklearn.neighbors.

![mnist_image](./wide_mnist.png)
