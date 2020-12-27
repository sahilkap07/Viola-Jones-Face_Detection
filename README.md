# Viola-Jones-Face_Detection

The video https://www.youtube.com/watch?v=uEJ71VlUmMQ&ab_channel=Computerphile explains the concept of face detection very well and can be helpful to understand the implementation.

# Training (Already Implemented - can skip this part):
This link http://vis-www.cs.umass.edu/fddb/ can be used to download the dataset. However for the purpose of this implementation, all the data is already attached in the files train_posf and train_negf which are the face data and non-face data respectively. The extracted face and non-face data can be used to train the classifier using Haar features as explained below.

How to run
Run (training): Train a cascaded classifier by following the given steps:

extract "train_posf" and "train_negf" files
Run "haar_features.py" to extract all possible haar feature values for each images in positive and negative face images
Run "threshold_optimization.py" to get optimized thresholds for each weak classifier(haar feature)
Run "ada_boost.py" to get the most relevant weak classifiers(haar features), that give minimum error on classifying positive and negative face images, for faces in sequence
Run "cascade_training.py" to build a cascade out of the relevant weak classifiers extracted from adaboost.
Run (for detection): Can use already trained cascade for detection purpose
1. Extract "train_posf" and "train_negf" files. 
2. Run "haar_features.py" to extract all possible haar feature values for each images in positive and negative face images.
3. Run "threshold_optimization.py" to get optimized thresholds for each weak classifier(haar feature).
4. Run "ada_boost.py" to get the most relevant weak classifiers(haar features), that give minimum error on classifying positive and negative face images, for faces in sequence.
5. Run "cascade_training.py" to build a cascade out of the relevant weak classifiers extracted from adaboost.
6. Run (for detection): Can use already trained cascade for detection purpose.

# Detect Faces:
Run "FaceDetection.py" followed by a space and <..relative directory to the images to be detected>.

# For further explanation regarding training process and implementation, please refer to the attached report.
