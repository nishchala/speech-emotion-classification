# Human emotion detection from speech

- This project works on the problem of identifying human emotions from speech samples. The aim is to experiment with various methods of classifying emotions and better understand the most distinctive features of emotions

## Required Dependencies

- numpy
- librosa
- tensorflow
- keras
- sklearn
- os
- matplotlib

## Dataset

Dataset used is Speech audio-only files (16bit, 48kHz .wav) from the RAVDESS. It contains 1440 files that include the Speech emotions - calm, happy, sad, angry, fearful, surprise, and disgust expressions.

## Steps to run

- Load data

  - Run the Data_creation.ipynb file to extract features from the audio files and generating test, train, validation csv files
  - Training and testing on scaled features using MinMaxScaler is also performed in Data_creation.ipynb file. csv files for scaled data set are created

- Train and test model

  - Run the model files ( ex. KNN_n.ipynb,LogisticRegression.ipynb ) for training and testing the models against the dataset

## Conclusions -

- Feature scaling seems to improve performance than non-scaled features.
- Ensemble model has the highest accuracy than any of the other models tested.

## Future Scope -

- Train and test Deep learning model to test the audio data
- Need to consider various methods like augmentation and test its impact on model performance
