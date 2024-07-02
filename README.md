**Problem Statement: Facial Expressions Recognition (FER)**   
Given images of human faces showing different expressions, the model should be able to categorise each image into one of 7 categories, each representing a facial expression (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).
- Model input: image - vector of pixels for a 48x48 pixel grayscale image
- Model output: Number from 0 to 6 which indicates the facial expression illustrated in the image
  
**Evaluation:**
Weighted accuracy metric is used to account for class imbalance

**Selected Dataset:**
FER2013 Dataset

**Baseline Model:** 
VGGNet, short for Visual Geometry Group Network, trained on FER2013 dataset achieving an accuracy of 73.28%. It is a classical CNN consisting of 4 convolutional stages and 3 fully connected layers.   
<img width="355" alt="image" src="https://github.com/Masa-Tantawy/Facial-Expression-Recognition/assets/81775839/f3f1e6dd-0275-44ec-b365-c5cf1d6e3415">

**Methodology:**
- Hyperparameters Tuning
- Data Imbalance Handling
- Data Augmentation
- Auxiliary Data
- Ensemble Model
- Real-time classification application
  
**Final Model:**   
Final Output = average output of 3 distinct VGGNet models → ROS, SMOTE, SmoteTomek (augmented and auxiliary data excluded as they deteriorated the model).
- Top-1 Accuracy: 97.18%
- Top-2 Accuracy : 99.58%
- Top-3 Accuracy : 99.72%

**Dependencies:**
- Pandas
- Numpy
- Seaborn
- Matplotlib
- Keras TensorFlow
- sklearn
- imblearn
- imgaug
- imageio
- os
- cv2   
All required dependencies are imported in the notebook.
The model weights can be found [here](https://drive.google.com/drive/folders/1k_BRhO_E7dmuGrKZY_HquU3OME1UsUiX?usp=drive_link) 
