# Head_Pose_Estimation
Head Pose Estimation using Mediapipe and CV - SVM, Random Forest

### Our Problem is that we are going to estimate the head pose from some key points on our face 

### what is the pose estimation ?
- #### the pose of an object refers to its relative orientation and position with respect to a camera. You can change the pose by either moving the object with respect to the camera, or the camera with respect to the object.
- #### The pose estimation problem described in this tutorial is often referred to as Perspective-n-Point problem or PNP in computer vision jargon. As we shall see in the following sections in more detail, in this problem the goal is to find the pose of an object when we have a calibrated camera, and we know the locations of n 3D points on the object and the corresponding 2D projections in the image.

### How to mathematically represent camera motion ?
- ### 3D Object has only two kinds of motions
##### 1-Translation: Moving the camera from its current 3D location (X, Y, Z) to new 3D Location (X', Y', Z') ==> Eqn.: ( X' - X, Y' - Y, Z' - Z )
##### 2- Rotation: You can also rotate camera about X, Y and Z axes

##### You can represent it using Euler angles ( roll, pitch and yaw ), 
##### a 3 * 3 rotation matrix, or a direction of rotation (i.e. axis ) and angle.

### What do we need for pose estimation?
##### 1- 2D coordinates of a few points : (x,y) locations for a few points in the image 
##### 2- 3D coordinates of same points: reference but we really don't implement 3D Model
##### 3- Intrinsic parameters of the camera: you need to know the focal length of the camera, the optical center in the image and the radial distortion parameters

### Our Steps ?
##### 1- Read Dataset using Mediapipe from jpg files
##### 2- Read 3 Euler Angles from Mat File in Dataset (Pitch, Yaw, Roll)
##### 3- Prepare and Explore Data Features
##### 4- Preprocess Data (Normalize)
##### 5- Split Data
##### 6- Train Models
##### 7- Test and Evaluate Models
##### 8- Test on Videos

### Required libraries

- Numpy
- Pandas
- Mediapipe
- cv2
- os
- sklearn

### Test Video

https://user-images.githubusercontent.com/44030209/174431141-d1833252-35c8-4d46-9481-be2049844135.mp4


