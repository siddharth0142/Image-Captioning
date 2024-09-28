# Image-Captioning

This project demonstrates how to generate image captions using a deep learning model combining VGG-16 for image feature extraction and RNN (Recurrent Neural Network) for caption generation. The captions are then converted into audio output.

### Table of Contents
1. Overview
2. Workflow
3. Installation
4. Model Architecture
5. Evaluation Metric

## Overview

This project takes an image as input and generates a meaningful caption that describes the content of the image. The caption is generated using a combination of Convolutional Neural Networks (CNN) for extracting image features and Recurrent Neural Networks (RNN) for processing sequential data, in this case, the image captions.

Finally, the generated caption is converted into speech as audio output.

## Workflow 

Below is the general workflow of the system:

1. Input Image:
The process starts with providing an input image.
  
3. Image Captioning Process:
The image is passed through a pre-trained VGG-16 model to extract the features. The features are then processed using an RNN model to generate captions.

4. Audio Output:
The generated caption is transformed into audio output


## Installation

1. Clone the repository
   * git clone https://github.com/siddharth0142/Image-Captioning.git
2. Install dependencies
   * TensorFlow / Keras
   * OpenCV
   * NumPy
   * Text-to-Speech (TTS) Library
   * NLTK (for tokenization)
 
## Model Architecture
  * VGG-16:
  A pre-trained VGG-16 model is used for extracting features from the input images. This acts as the encoder part of the image captioning system.
  
  * RNN (LSTM/GRU):
  The extracted features from the VGG-16 model are passed to an RNN model (LSTM/GRU) to generate a sequence of words that form a descriptive caption for the image.

![image](https://github.com/user-attachments/assets/361f2f5a-a425-4e24-a16b-4302ce4fc117)

## Evaluation Metric

BLEU Score:
 * BLEU compares the generated captions with reference captions based on n-gram matches.
 * It evaluates how well the generated captions match the human-written captions by measuring the overlap of words or phrases between the generated and reference captions.
