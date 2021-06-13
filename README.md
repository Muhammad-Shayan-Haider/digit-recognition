# digit-recognition
Digit recognition done using two famous learning algorithms, feed forward artificial neural network and k nearest neighbour

**Dataset details**

MNIST images dataset is used for training and testing dataset for 2 learning models. Preprocessing is applied on the dataset, then models are used for classification and prediction. In pre-processing, grayscale images are normalized i.e. their pixel values are divided by 255 so we get each pixel value between 0 and 1. Furthermore, images are flattened from array of 28 x 28 pixels to 784 1-d array so that they can easily be analysed. 

**kNN Classifier**

It is an unsupervised learning algorithm which classifies data without providing it with the label data. Training data that was used had 54000 images and 6000 images for validation data. For different values of k, kNN algorithm was executed on validation data. The highest accuracy k value came out to be 3.

![image](https://user-images.githubusercontent.com/60185211/121812489-5abb3d80-cc81-11eb-9c5a-bd6160087804.png)

**FFANN classifier**

Feedforward artificial neural network is an artificial neural network in which connections do not form a cycle. The model that is used is a multi-layer perceptron having 3 layers, 1 input layer with activation function of tanh having 256 neurons, 1 hidden layer having 37 neurons and relu as activation function, and finally output layer has 10 neurons and activation function of softmax. The optimizer, for the compilation of the model, we used is adam. Then model is trained over 25 epochs and 64 samples per gradient update.
The accuracy of FFANN is 97%. Some sample results of FFANN.

![image](https://user-images.githubusercontent.com/60185211/121812616-e7fe9200-cc81-11eb-89d5-9c1f12daebf5.png)
