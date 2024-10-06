# ImageCaptioning with CNN LSTMs
This repository contains code for generating descriptive captions for images using a deep learning model that combines a Convolutional Neural Network (CNN) with a Long Short-Term Memory (LSTM) network.

## Key features and functionalities:

* Image preprocessing: Handles image resizing, normalization, and other necessary preprocessing steps.
* CNN (ResNet) architecture: Implements a ResNet model to extract deep features from the image.
* LSTM model: Utilizes an LSTM network to generate the textual caption sequence.
* Training and evaluation: Provides scripts for training the model on a labeled dataset and evaluating its performance using metrics like perplexity.
* Inference: Demonstrates how to use the trained model to generate captions for new images.

### Image Encoder 

ResNet-152 (https://arxiv.org/abs/1512.03385) is a deep convolutional neural network (CNN) architecture that has achieved state-of-the-art performance on various computer vision tasks, including image classification, object detection, and semantic segmentation. Its depth and residual learning mechanism allow it to capture complex patterns and features in images effectively.   

Key Features
* Residual Learning: ResNet-152 incorporates residual learning blocks, which enable the network to learn residual functions instead of the entire underlying mapping. This helps to alleviate the vanishing gradient problem and allows for the training of very deep networks.
* Depth: With 152 layers, ResNet-152 is a very deep network, allowing it to capture intricate patterns and details in images.
* Pre-trained Weights: ResNet-152 is often used with pre-trained weights on the ImageNet dataset, providing a strong feature extractor for various tasks.


![image](https://github.com/user-attachments/assets/ac08d163-d32e-4d65-aa03-f4fea3c03fdb)

### Decoder : LSTM for generation textual caption

Long Short-Term Memory (LSTM) networks are a type of recurrent neural network (RNN) specifically designed to address the vanishing gradient problem that can occur in traditional RNNs, making them well-suited for tasks involving sequential data, such as language modeling and image captioning.

How LSTM Works
LSTMs introduce a concept called "gates" to control the flow of information through the network. These gates include:

* Input gate: Determines how much of the new input should be remembered.
* Forget gate: Controls how much of the previous state should be forgotten.
* Output gate: Determines how much of the internal state should be output.
This gated architecture allows LSTMs to effectively handle long-range dependencies in the data, making them suitable for tasks where the output depends on information from earlier parts of the sequence.

## Requirements 

Python
PyTorch 
NumPy
Other necessary libraries (e.g., nltk, tqdm)
