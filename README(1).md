
# Head Pose Estmiation


Used a training dataset contains of 2000 face
images, each image has 3 different output
angles for each dimension.
Extracted features, using MediaPipe, as 468
point from the face.
Created 3 different models to predict each
angle of the 3 angles, each model was chosen
from a precise Grid-search.
Applied these models on the test images and
achieved a MSE around 10% for each model of
the 3.
Applied them on videos by splitting them into
frames, each frame is used to extract the 468
points from the face by MediaPipe library and
feed them to the model which can predict the 3
angels and draw the axes accurately.
## Roadmap

- Installing MediaPipe
- Required Libraries
- Dowloading Data
- helper functions
- Preparing Data
- Checking how many images Mediapipe actually captuerd
- Stacking points into array
- Centering the points at index 99
- Choosing the distance between 2 random points and divide all points by that distance
- Splitting the dat and importing diffrent models
- Cross Validtaion for the three angels to know which model is the best between SVR & XGBRegressor
- Fitting the best models and observing their MAE
- Comparison between Orgininal Axis & Predicted Axis
- Using the models to estimate poses from a new video by applying them on frame by fame
- converting the frames to video


