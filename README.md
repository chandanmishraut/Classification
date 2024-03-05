# Classification
Machine Learning and Deep Learning models for Classification

This code performs a machine learning task using a neural network to classify beans based on various features. Here's a summary of the key steps:

Data Preparation: The code reads data from a CSV file containing information about beans. It preprocesses the data by dropping certain columns and splitting it into training, validation, and test sets.

Data Scaling and Encoding: The features are scaled using StandardScaler, and the target labels are encoded using LabelEncoder. Oversampling is applied to the training data using RandomOverSampler to handle class imbalance.

Neural Network Model: The code defines a neural network model using TensorFlow's Keras API. The model architecture consists of multiple dense layers with ReLU activation, followed by a softmax output layer. The model is compiled with the Adam optimizer and sparse categorical crossentropy loss.

Training and Validation: The model is trained using the training data, with validation data used for monitoring performance. Training is performed for multiple epochs with a batch size of 64.

Model Evaluation: After training, the best model based on validation loss is selected. The performance of this model is evaluated on the test set using classification metrics such as precision, recall, and F1-score for each class, as well as overall accuracy.

Visualization: The code includes a function to plot the training and validation loss, as well as accuracy, over epochs to visualize the model's performance during training.
