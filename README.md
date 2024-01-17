# ConvolutionalNN_MNIST-classification
This Python script demonstrates the implementation of a convolutional neural network (CNN) using TensorFlow and Keras for the MNIST digit classification task.

Here's a brief description of the code:

Model and Data Parameters:
Specifies the number of classes (digits 0-9) and the input shape for the images (28x28 pixels with one channel).

Data Loading and Preprocessing:
Loads the MNIST dataset, consisting of handwritten digit images and their corresponding labels.
Scales the pixel values of the images to the [0, 1] range.
Expands the dimensions of the images to include a single channel.

Model Definition:
Constructs a sequential model using Keras with the following layers:
Convolutional layer with 32 filters and ReLU activation.
MaxPooling layer.
Convolutional layer with 64 filters and ReLU activation.
MaxPooling layer.
Flattening layer.
Dropout layer with a dropout rate of 0.5.
Dense layer with softmax activation for the output.

Model Compilation:
Compiles the model using categorical crossentropy loss, the Adam optimizer, and accuracy as the evaluation metric.

Model Training:
Trains the model on the training data with a batch size of 128 and 15 epochs.
Includes a validation split of 10% for monitoring training performance.

Model Evaluation:
Evaluates the trained model on the test data.
Prints the test loss and accuracy.

The code provides a concise implementation of a CNN for recognizing handwritten digits from the MNIST dataset, showcasing common practices in deep learning model development using TensorFlow and Keras.
