# Hand gesture classification
The main motivation of this project is to approach the challenge of human activity recognition (HAR), in particular hand gestures. The solution is inspired by skeleton-based models of the hand, which use 3D locations of the joints in RGB-D images as observable features of human gestures. The designed deep neural network predicts dynamic hand gestures from 3D coordinate series. It is also built a model which 2D coordinates to evaluate the impact of the depth coordinate in the results.

## Gesture classes
The dataset is composed of 5 different gestures:
* WAVING                        
* SCISSORS
* FLIP
* PUSH&PULL
* OPEN&CLOSE

![Image 1](/images/WAVING.gif) ![Image 2](/images/SCISSORS.gif) ![Image 3](/images/FLIP.gif) ![Image 4](/images/PUSH&PULL.gif) ![Image 5](/images/OPEN&CLOSE.gif)

## Technologies
Project is created with:
* Tensorflow 2.0
* Scikit-Learn
* Pandas
* Numpy
* Matplotlib

## Proyect structure
The workflow consists of the following steps:
1. Gathering data [code](/GatheringData.ipynb)
2. Data preparation [code](/DataPreparation.ipynb)
3. Model selection
4. Model Training
5. Models Evaluation [code](/3DModel.ipynb) [code](/2DModel.ipynb)

## References
The hand keypoint coordinates are detected using the source code of the following paper:
* Y. Wang, B. Zhang, C. Peng,"SRHandNet: Real-Time 2D Hand Pose EstimationWith Simultaneous Region Localization", IEEE, Transactions on Image Processing,Volume 29, Pages 2977 - 2986, DOI:10.1109/TIP.2019.2955280, 2019.
