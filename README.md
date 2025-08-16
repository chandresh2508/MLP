# MLP
MLP Final Project
Lightweight CNN for Text Classification
This repository contains the code for a final project for AIDI 1002, focusing on text classification using a lightweight Convolutional Neural Network (CNN). The project demonstrates a full machine learning pipeline from data preprocessing to model training and evaluation on the AG_NEWS dataset.

1. Project Overview
The primary goal of this project is to implement an efficient text classification model. We've developed a custom Lightweight CNN and evaluated its performance on the task of categorizing news articles into one of four classes: World, Sports, Business, and Sci/Tech.

This implementation serves as a significant contribution to a standard text classification methodology by introducing a specialized, compact CNN architecture designed for effectiveness without the high computational cost of larger, more complex models.

2. Dataset
The project uses the AG_NEWS dataset, which is a collection of more than 1.3 million news articles. The version used in this project is a subset containing 120,000 training samples and 7,600 test samples, distributed across four categories. The dataset is automatically downloaded via the Hugging Face datasets library, so no manual download is required.

3. Getting Started
Prerequisites
To run this code, you need to have Python and pip installed. The project's dependencies can be installed using the following command:

Bash

pip install torch datasets scikit-learn
File Structure
The entire project code is contained in a single file, lightweight_cnn.py.

Running the Code
Simply execute the Python script from your terminal:

Bash

python lightweight_cnn.py
The script will automatically perform the following steps:

Load and preprocess the AG_NEWS dataset.

Build the vocabulary and prepare the data loaders.

Initialize and train the Lightweight CNN model.

Evaluate the model on the test set.

Print the training progress and final performance metrics.

4. Results
The model was trained for 5 epochs, showing consistent improvement in training loss. The final performance on the unseen test set demonstrates the effectiveness of the lightweight architecture.

Training Progress
The following table shows the training loss at the end of each epoch:

Epoch	Train Loss
1	0.584
2	0.315
3	0.243
4	0.197
5	0.163

Export to Sheets
Final Performance on Test Set
Metric	Value
Test Loss	0.306
Test Accuracy	0.909
Test F1 Score	0.909

Export to Sheets
The results indicate that the Lightweight CNN successfully learned to classify news articles with a high degree of accuracy, achieving an excellent F1 score of over 90%. This confirms that the model is both effective and well-generalized.
