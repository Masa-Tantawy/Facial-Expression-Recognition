**Problem Statement: Facial Expressions Recognition (FER)**   
Given images of human faces showing different expressions, the model should be able to categorise each image into one of 7 categories, each representing a facial expression. These are: 0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).
- Model input: image - vector of pixels for a 48x48 pixel grayscale image
- Model output: Number from 0 to 6 which indicates the facial expression illustrated in the image
To evaluate the model effectiveness, the weighted accuracy metric is used, which accounts for class imbalance in the data.

**Selected Dataset: FER2013**

Baseline Model - VGGNet, short for Visual Geometry Group Network
- Training: FER2013 dataset achieving an accuracy of 73.28% 
A classical CNN consisting of 4 convolutional stages and 3 fully connected layers.
<img width="355" alt="image" src="https://github.com/Masa-Tantawy/Facial-Expression-Recognition/assets/81775839/f3f1e6dd-0275-44ec-b365-c5cf1d6e3415">

Methodology
- Hyperparameters Tuning:
