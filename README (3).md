# Sarcasm-Detection-using-TensorFlow-and-Keras
This project is focused on detecting sarcasm in textual data using Natural Language Processing (NLP) techniques. The model is built using TensorFlow and Keras, and it aims to classify whether a given sentence is sarcastic or not.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Applications](#applications)
- [Results](#results)
- [Contact](#contact)

## Overview

Sarcasm detection is a challenging task in NLP due to the nuanced nature of sarcasm. The goal of this project is to build a model that can accurately classify sentences as sarcastic or non-sarcastic. The project utilizes a deep learning approach with a focus on sequence models.

## Dataset

The dataset used for training and testing the model consists of labeled sentences indicating whether they are sarcastic. The data is tokenized and preprocessed to feed into the neural network. It has been retrieved using the Google API.

## Model Architecture

The model used in this project is a sequential neural network with the following layers:

1. **Input Layer:** Accepts input sequences of length 100.
2. **Embedding Layer:** Converts words into dense vectors of size 128.
3. **Bidirectional LSTM Layer:** Processes the input sequence in both directions, resulting in an output of shape `(None, 100, 256)`.
4. **Self-Attention Layer:** Applies attention mechanism to focus on important parts of the sequence.
5. **Global Average Pooling Layer:** Reduces the dimensionality by computing the average over the sequence length.
6. **Flatten Layer:** Flattens the output from the pooling layer to a 1D vector.
7. **Dense Layer 1:** Fully connected layer with 256 units.
8. **Dense Layer 2:** Fully connected layer with 128 units.
9. **Dense Layer 3:** Fully connected layer with 64 units.
10. **Dropout Layer:** Adds dropout regularization with a dropout rate to prevent overfitting.
11. **Dense Layer 4:** Final output layer with a single unit for binary classification.

The model was trained using a binary cross-entropy loss function and the Adam optimizer.

## Results

**Sentence**: "poor man becomes PM" | Prediction: 0.8487 (Sarcastic)

**Sentence**: "This session was amazing" | Prediction: 0.0362 (Non-Sarcastic)

## Applications

- **Social Media Monitoring:** Improve brand reputation management and content moderation.
- **Customer Support:** Enhance automated response systems and sentiment analysis.
- **Market Research:** Gain accurate consumer insights and refine product development.
- **Opinion Mining:** Analyze public opinion and survey responses accurately.
- **Content Recommendation Systems:** Personalize content and refine ad targeting.
- **Human-Computer Interaction:** Improve virtual assistants and interactive systems.
- **Content Creation and Curation:** Manage sarcastic tones in writing and curate content.
- **Legal and Forensic Analysis:** Assist in e-discovery and cybersecurity investigations.

## Contact
- LinkedIn: [Zainab Siddiqui][https://www.linkedin.com/in/siddiquizainab/]
