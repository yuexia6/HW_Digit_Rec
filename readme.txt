#HW_Digit_Rec
This project is a simple test for utilizing html,css,javascript,python,tensorflow,etc for testing the connection (using cgi) between front-end and back-end, with basic machine learning method (using tensorflow framework) to recognize handwritten one digit (offline recognization).

# Python
Python 3.5+ is utilized. As there're multiple versions of python installed on my mac, first line like:"#!/Library/Frameworks/Python.framework/Versions/3.5/bin/python3" are necessary to set the default version to python3.

# Required modules
can simply install by:
pip install -r requirements.txt


# How to use locally
To launch the website:
python -m http.server --cgi ****
(**** can be your choice of 4 digits, for example 8888)

Then navigate to `http://localhost:****/index.html` (like 0.0.0.0:8888) to use this website. (Firefox/Chrome is better)


# Machine Learning Model
define_model.py:
A convolutional neural network (CNN) is defined within the "define_model.py" module using the TFLearn library. 

train_model.py:
The defined CNN can be trained against the MNIST dataset by running the "train_model.py". 

mnist.py:
Implements the trained model against the user's hand-drawn input and output the prediction of each digit.

#Limitation:
As teh habits of writting digits are different from each other regions, especially compare "7" in US and China, which is very different, as the mnist dataset was collected in the habit of US., writing digits in US habit will help/improve the accuracy of recognization.

-- Yue Xia Augest 2018
