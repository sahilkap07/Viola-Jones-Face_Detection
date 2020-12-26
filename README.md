# Viola-Jones-Face_Detection

How to run
Run (training): Train a cascaded classifier by following the given steps:

extract "train_posf" and "train_negf" files
Run "haar_features.py" to extract all possible haar feature values for each images in positive and negative face images
Run "threshold_optimization.py" to get optimized thresholds for each weak classifier(haar feature)
Run "ada_boost.py" to get the most relevant weak classifiers(haar features), that give minimum error on classifying positive and negative face images, for faces in sequence
Run "cascade_training.py" to build a cascade out of the relevant weak classifiers extracted from adaboost.
Run (for detection): Can use already trained cascade for detection purpose

Run "FaceDetection.py" followed by a space and <..relative directory to the images to be detected>.
