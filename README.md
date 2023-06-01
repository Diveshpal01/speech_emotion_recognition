**Voice Emotion Classification**

This repository contains code for classifying emotions in voice recordings using the RAVDESS dataset. The code uses the librosa library to extract features such as MFCC, chroma, and mel from sound files, and then trains a Multi-Layer Perceptron (MLP) classifier to predict the emotions.

**Prerequisites**

Python 3.x
Required Python libraries: librosa, soundfile, numpy, scikit-learn

**Code Explanation**

The code is divided into several parts:

Feature Extraction: The extract_feature function is responsible for extracting MFCC, chroma, and mel features from a sound file using the librosa library.

Emotions Mapping: The emotions dictionary maps emotion codes to their corresponding labels.

Emotions to Observe: The observed_emotions list contains the emotions to be considered for classification.

Data Loading: The load_data function loads the sound files from the specified directory, extracts features using the extract_feature function, and prepares the data for training and testing. It returns the training and testing datasets.

Dataset Split: The data is split into training and testing sets using the train_test_split function from scikit-learn.

Model Training: The MLP classifier model is initialized and trained using the training dataset.

Model Evaluation: The model is evaluated on the testing dataset by predicting the emotions and calculating the accuracy using the accuracy_score function.

Results: The accuracy of the model and the predicted emotions are printed.

**Results**

After running the code, the following results are displayed:

Training set shape: (414, 180)
Testing set shape: (138, 180)

Accuracy: 92.03%

Predicted emotions: [emotion1, emotion2, ...]
