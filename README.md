# A simple test project of image classification

In this project, the primary objective is to utilize scikit-learn for a straightforward image classification task. More importantly, the focus lies on the conclusions drawn from altering neural network parameters. 

The code description is in the Juyter notebook file.


## Conclusion

The sklearn package provides us with a dataset for training our network. It offers an array of matrices along with their corresponding targets. Additionally, it includes a series of attributes for each set of images, such as the target label. Therefore, our training dataset is represented as a three-dimensional matrix. The first two dimensions, 8x8, represent the 64 pixels of each image, while the third dimension corresponds to the number of these matrices, totaling 1797. In the code, the matplotlib package is utilized to visually represent these matrices.

When dealing with larger images, say with 400 pixels, the input layer consists of 400 neurons.**Consequently, there arises a necessity to increase the number of hidden layers to effectively extract features from the images.** The output layer remains unchanged and is responsible for classifying the images into categories ranging from 0 to 9.

**In the subsequent step, the same dataset is employed, with the first 1000 samples allocated for training and the remainder for testing. For each of these samples, whether utilized for training or testing, the corresponding targets are assigned to the variable y.**

**Increasing the number of neurons in the hidden layer typically enhances accuracy. For instance, setting it to 50 results in an accuracy of 94%. However, excessive increase might not necessarily lead to improved accuracy. For instance, setting it to 120 yields an accuracy of 93%.**

**Conversely, decreasing the learning rate too much tends to decrease accuracy. Conversely, raising the learning rate, such as to 0.7, unexpectedly decreases accuracy to around 80%.**

**When the activation function is set to Relu, accuracy significantly declines, indicating it's not an optimal choice, with accuracy falling below one percent. However, using tanh results in similar performance to sigmoid.** 
