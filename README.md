😃 Speech Emotion Detection Using MFCC and CNN
This project detects emotions from speech audio clips using 
**MFCC (Mel-Frequency Cepstral Coefficients)** for feature 
extraction and a **CNN (Convolutional Neural Network)** for classification.

🎯 Objective
Given an audio clip of a speaker, the model predicts the **emotion** 
being expressed, such as _happy, sad, angry, neutral_, etc.

🚀 Features
(i)Loads and preprocesses raw audio files
(ii)Extracts MFCCs as features from speech
(iii)Trains a CNN to classify emotions
(iv)Supports multi-class emotion classification
(v)Evaluates performance with metrics and visualizations

🧠 Technologies Used
(i)Python
(ii)librosa – audio processing and MFCC extraction
(iii)numpy, pandas – data handling
(iv)matplotlib, seaborn – for plots
(v)tensorflow / keras – CNN modeling

Recommended: Use open datasets like [RAVDESS](https://zenodo.org/record/1188976) or [TESS](https://tspace.library.utoronto.ca/handle/1807/24487).

## 🛠 How It Works

1. **Audio Preprocessing**:

   * Loads `.wav` files using `librosa`.
   * Extracts 40 MFCCs per clip.
   * Pads or truncates to ensure uniform input shape.

2. **Model**:

   * A Convolutional Neural Network (CNN) that learns patterns from MFCCs.
   * Final layer uses `softmax` for multi-class emotion classification.

3. **Training**:

   * Split data into train/test sets.
   * Monitor accuracy and loss over epochs.

4. **Evaluation**:

   * Prints test accuracy.
   * Optionally plots a confusion matrix and loss/accuracy graphs.


## ⚠️ Notes

* All audio files should be:

  * Mono-channel
  * Same sampling rate (e.g., 22050 Hz)
* Model performance depends on:

  * Dataset quality
  * Audio clarity
  * Emotion labeling consistency
* You may enhance accuracy using:

  * Data augmentation (noise, pitch shift)
  * More complex models (e.g., CRNNs, LSTMs)

