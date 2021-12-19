# Classification Model for Face Recognition
-----
### About the project
This project is a classification problem using scikit-learn library of recognizing faces of 40 different people in 400 images. 
There are many machine learning models for these kind of problems, but I found the best model that fits this problem 
and I also found hyperparameters that brought high accuracy. 

-----
### Scikit-Learn Installation
This project uses scikit-learn. 
If you haven't installed scikit-learn, install scikit-learn in your jupyter notebook through the code I mentioned below.
```sh
!pip install scikit-learn
```
-----
### About the Dataset
###### This dataset contains a set of face images`_ taken between April 1992 and April 1994 at AT&T Laboratories Cambridge.
###### There are ten different images of each of 40 distinct subjects. For some subjects, the images were taken at different times, varying the lighting,
###### facial expressions (open / closed eyes, smiling / not smiling) and facial details (glasses / no glasses). 
###### All the images were taken against a dark homogeneous background with the subjects in an upright, frontal position (with tolerance for some side movement.
###### The image is quantized to 256 grey levels and stored as unsigned 8-bit integers; the loader will convert these to floating point values on the 
###### interval [0, 1], which are easier to work with for many algorithms.
###### The "target" for this database is an integer from 0 to 39 indicating the identity of the person pictured; however, with only 10 examples per class, this
###### relatively small dataset is more interesting from an unsupervised or semi-supervised perspective.
###### The original dataset consisted of 92 x 112, while the version available here consists of 64x64 images.
-----
### Logistic Regression
I found out logistic regression is the best model for face recognition. Since logistic regression is used to model the probability of a certain class or event
and this can be extended to model several classes of events such as determining whether an image contains a cat, dog, lion, etc, this fits this project which 
is recognizing faces of people. 
-----
### Hyperparameter I used
In this project I've changed C and random_state. C is an inverse of regularization strength and it has smaller values specify stronger regularization.
But since hyperparameter defers every project, in this project increasing the value of C to 100 increased the accuracy of the project. 
Also, I've changed random_state into 0 since not changing random_state into 0 changes the accuracy everytime I execute the project. 
Fixing the value of random_state into 0 can make the accuracy stay the same.
Through chaning these two hyperparameters, accuracy increased to 97%.
```sh
C = 100
random_state = 0
```
