# Preprocessing with training and testing data
When preprocessing data, the data preprocessing should be done first on the training data without the testing data then applied to the testing data. In my case, this means that the PCA should be done with the training data and the testing data should be projected into the PCAs found with only the training data. This is explained [here](https://stats.stackexchange.com/questions/55718/pca-and-the-train-test-split). Likewise the data normalization should be found with the training set and then applied to the testing data when the model is evaluated. This is explained in [this post](https://stats.stackexchange.com/questions/77350/perform-feature-normalization-before-or-within-model-validation).