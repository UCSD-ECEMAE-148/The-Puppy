<h1 align="center">MAE 148 Team 4 Final Project: The Puppy</h1>

<h1 align="center">Summer Session 2, 2024</h1>

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/3387eed61e11feb096777f3d9380c218c35fbe62/images%20and%20video/Extra%20delivarables/Us.jpg" width="700" height="600"></p>

[![Video of final project]()


### Team members (from left to right):

- Yutao Deng (Mechanical Engineering) 

- Adam Ornelas (Mechanical Engineering)

- Niran Cuevas (Aerospace Engineering)


### Timeline of our final presentation:

On August 27th 2024 we proposed the idea of training our robot to follow a specific person while simultaneously being able to respond to commands given by said person. We initially proposed training our own model so that our robot could identify specific geometric shapes in order to accomplish this. To do so, we first captured images of simple signs. Using these images we were able to annotate our own personal dataset for training using Roboflow. Below you can see some of these images:

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/c597bcfa7655a614abad8d3a6b0a2e31d45a0b78/images%20and%20video/Signs/Proposed%20Signs%201.png" width="700" height="600"></p>
<p align="center">**Proposed Signs 1**
  
We decided to use Roboflow because it is a very versatile website that allows you to train custom models, source annotated datasets for training, and/or find datasets with models that are already trained. Roboflow is a really great resource for finding and implementing computer vision models on a number of devices which includes the OAK-D camera we have on our car. We learned to make sure to source a model with the model type YOLO v8 when using an OAK-D camera. This ensured that the camera could communicate with the model via the ROS2 package we later installed onto our NVIDIA Jetson Nano. 
