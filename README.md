Here's a README section you can use for your project:

---

# Gender Prediction Model

This project involves training a gender prediction model using names as input. The model predicts whether a given name is more likely to be male or female. The model is trained using TensorFlow and Keras, with a dataset of 95,024 names labeled as male or female.

## Dataset

The dataset used for training consists of two columns:
- Names: A list of names.
- Gender: The corresponding gender for each name ('M' for Male, 'F' for Female).

# Preprocessing

- Names are converted to lowercase to ensure uniformity.
- The gender labels are converted to binary values: 0 for Male and 1 for Female.
- The names are vectorized using a `CountVectorizer` with character-level n-grams (ranging from 1 to 3 characters).

# Model Architecture

The model is a simple feedforward neural network with the following layers:
- **Dense Layer**: 128 units, ReLU activation
- **Dense Layer**: 64 units, ReLU activation
- **Dense Layer**: 1 unit, Sigmoid activation (for binary classification)

# Training

- The model is trained for 20 epochs with a batch size of 32.
- The training data is split into 80% for training and 20% for validation.
- The model achieves an accuracy of approximately 89.57% on the test set.

# Model Usage

To use the trained model for gender prediction:

1. Load the model and vectorizer.

2. Predict the gender of a new name.
 

# Dependencies

- pandas
- tensorflow
- scikit-learn
- joblib

