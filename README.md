# Behavioral Cloning Project

[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---
The objective of this project is to train the computer to drive the car on the tracks provided by Udcity simulator. The computer needs to be trained using the simulator images provided by udacity. The concepts of Deep Learning and Convolutional Neural Networks are applied here to make the car drive safely and autonomously through the track. 

The model is trained by feeding the data gathered from simulator in the form of images captured from three dashboard cameras left, center and right. This training data has a assciated ground truth labels which are stored in csv file and it contains mappings of left, center and right images and the corresponding steering angle, throttle, brake and speed. 

Using Keras Deep learning framework we can create a ".h5" file which we can test later on simulator. The challenge in this project is to collect all types of training data and train the model so that it will respond correctly to all types of scenes on track without overfitting and underfitting. 

Model Architecture and Training Strategy
---
After exploring different models like AlexNet, VGGNET I decided to go with the model from NVDIA. The model architecture is described in [a paper by Nvidia](http://images.nvidia.com/content/tegra/automotive/images/2016/solutions/pdf/end-to-end-dl-using-px.pdf).  
<img src="examples/NVIDIA.jpg" width="480" alt="NVDIA Model" />
