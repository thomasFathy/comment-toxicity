Comment Toxicity Detection using LSTM
This project implements a deep learning model for detecting toxic comments. It leverages TensorFlow and Keras to create a Bidirectional LSTM network for multi-label classification of comments into different categories of toxicity. The model is trained to predict six categories of toxic behavior such as threats, insults, and hate speech.

Table of Contents
Overview
Model Architecture
Requirements
Installation
Usage
Evaluation Metrics
Results
Contributing
License
Overview
The purpose of this project is to automatically classify comments as toxic or non-toxic across multiple categories. The model is designed to predict toxicity across six different labels, allowing for detection of both general and specific toxic behaviors.

The six categories of toxicity include:

Toxic
Severe Toxic
Obscene
Threat
Insult
Identity Hate
This multi-label classification task uses an LSTM network to capture sequential dependencies in text and make predictions about each comment’s toxicity level.

Model Architecture
The model is built using the following layers:

Embedding Layer: Converts words into dense vectors with a fixed size, which serves as input for the LSTM layer.
Bidirectional LSTM Layer: A layer that processes the input sequence in both forward and backward directions to better capture context.
Dense Layers: Fully connected layers for non-linear transformations. Three Dense layers with ReLU activations are used.
Sigmoid Output Layer: Outputs probabilities for each of the six categories of toxicity.

Requirements
The project requires the following libraries:
- Python 3.x
- TensorFlow 2.x
- Keras
- NumPy
- Pandas
- Scikit-learn

Evaluation Metrics
The model is evaluated using the following metrics:

Precision: The ratio of correctly predicted positive observations to total predicted positives.
Recall: The ratio of correctly predicted positive observations to all observations in the actual class.
Accuracy: The ratio of correctly predicted observations to the total observations.
These metrics are used to evaluate the performance of the model in detecting toxic comments.

Results
The model achieved the following performance metrics:

Precision: 0.79
Recall: 0.69
Accuracy: 0.47
These results show that the model performs reasonably well in predicting toxicity, though there is room for improvement in recall and accuracy.

Contributing
Contributions are welcome! If you have any improvements, feel free to submit a pull request or open an issue.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
