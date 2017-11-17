# Emotion recognition
A convolutional neural networks based project for facial expression recognition.
Built on top of openCV for computer vision and Keras-built CNN.

## CNN architecture
The neural network consists of: 
- One input layer in size of 48x48
- One convolutional layer with 52 filters and size of 48x48x52
- Pooling layer with 2x2 window with the size of 24x24x52
- Flat layer with 512 nodes
- Output layer of size 7x1

## Train data
The train data is the fer2013 dataset from kaggle.com facial expression recognition competition. 
The dataset is a .csv file with three columns:
1. Facial expression number (0 to 6)
2. 2304 space separated numbers from 0 to 255. It is the 48x48 grayscale image with gray color intensity.
3. Label that states whether this point if for train or test

The dataset consists of 35887 images of human faces with different emotions: neutral, sad, happy, disgust, fear, angry and surprise.

## Training
The training was performed on NVidia GeForce 740M GPU and took 102 seconds per epoch on average. All 20 epochs of training took near 35 minutes. The training accuracy was 95%. 
