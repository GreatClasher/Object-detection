![image](https://github.com/Shailly0502/Tech-Diwane/blob/5e9464e1145fa5ce5c6af266c36b0efb3198d7fa/activestatus.svg) ![python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white) ![micro](https://img.shields.io/badge/Microsoft_Learn-258ffa?style=for-the-badge&logo=microsoft&logoColor=white)![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white) ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Microsoft](https://img.shields.io/badge/Microsoft-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)![Bank of Baroda](https://github.com/Shailly0502/Tech-Diwane/blob/1d0c3ceafcb5ef858c117ddff4241770deaa5d2b/Bank%20of%20Baroda-Hackathon-orange.svg)![TechGig](https://github.com/Shailly0502/Tech-Diwane/blob/23028a580b78736f658e260fa1002a29068292ed/techgig.svg)  ![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white)![Deep Learning](https://github.com/Shailly0502/Tech-Diwane/blob/2d21b9fb791ddb4a8f74c0e65e394b6a568c0a6d/Deep-Learning-yellow.svg)![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white) ![Contributor](https://github.com/Shailly0502/Tech-Diwane/blob/cac5cd0b80f2648c84d53b58a081daacdf7bed2f/Tech%20Diwane-4-Green.svg) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) 

##Object Tracking using CNN and RNN. 

Followed the papers : Spatially Supervised Recurrent Convolutional Neural
Networks for Visual Object Tracking: https://arxiv.org/pdf/1607.05781.pdf and You Only Look Once:Unified, Real-Time Object Detection: https://arxiv.org/pdf/1506.02640.pdf

Dataset: http://cvlab.hanyang.ac.kr/tracker_benchmark/datasets.html


Designed a robust tracker which tracks appearance and motion over time.
Recurrent Neural Network (LSTMs) tracks the temporal information of the object and Convolutional Neural Network
(using YOLO) for Object Classification and bounding box prediction


The 4096 visual features obtained from YOLO Convolutional layer is concatenated with the 6 location coordinates of bounding boxes obtained after the fully connected layer of YOLO. 

These 4096 + 6 = 4102 features are given to stacked LSTM as input. 

With the help of visual features of the objects, the next location of the bounding boxes is predicted by the LSTM.
