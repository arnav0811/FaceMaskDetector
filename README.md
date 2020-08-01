## FaceMaskDetector

FaceMaskDetector is a classifier system using the Deep Learning technique called as Convolutional Neural Networks (CNN). This CNN Model is built using the TensorFlow framework and the OpenCV library which is highly used for real-time applications.FaceAttendance was costructed by Arnav Mardia for SmartnUp EdTech.

The Face Mask detection model is built using the Sequential API of the keras library. This allows us to create the new layers for our model step by step. The various layers used for our CNN model are described below.

 In this first step, the activation function used is the ‘ReLu’. This ReLu function stands for Rectified Linear Unit which will output the input directly if is positive, otherwise, it will output zero. The input size is also initialized as 150X150X3 for all the images to be trained and tested using this model

In the second layer, the MaxPooling2D is used with the pool size of 2X2.

The next layer is again a Conv2D layer with another 100 filters of the same filter size 3X3 and the activation function used is the ‘ReLu’. This Conv2D layer is followed by a MaxPooling3=2D layer with pool size 2X2.

In the next step, we use the Flatten() layer to flatten all the layers into a single 1D layer.

After the Flatten layer, we use the Dropout (0.5) layer to prevent the model from overfitting.

Finally, towards the end, we use the Dense layer with 50 units and the activation function as ‘ReLu’.

The last layer of our model will be another Dense Layer, with only two units and the activation function used will be the ‘Softmax’ function. The softmax function outputs a vector which will represent the probability distributions of each of the input units. Here, two input units are used. The softmax function will output a vector with two probability distribution values.

# Citations: 
Data - I have used the face mask dataset provided by Prajna Bhandary : https://www.linkedin.com/feed/update/urn%3Ali%3Aactivity%3A6655711815361761280/
https://towardsdatascience.com/covid-19-face-mask-detection-using-tensorflow-and-opencv-702dd833515b

