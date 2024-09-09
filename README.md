<h1 align="center">MAE 148 Team 4 Final Project: The Puppy</h1>

<h1 align="center">Summer Session 2, 2024</h1>

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/3387eed61e11feb096777f3d9380c218c35fbe62/images%20and%20video/Extra%20delivarables/Us.jpg" ></p>

### Team members (from left to right):

- Yutao Deng (Mechanical Engineering) 

- Adam Ornelas (Mechanical Engineering)

- Niran Cuevas (Aerospace Engineering)


### Timeline of our final presentation:

On August 27th 2024 we proposed the idea of training our robot to follow a specific person while simultaneously being able to respond to commands given by said person. We initially proposed training our own model so that our robot could identify specific geometric shapes in order to accomplish this. To do so, we first captured images of simple signs. Using these images we were able to annotate our own personal dataset for training using Roboflow. Below you can see some of these images:

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/c597bcfa7655a614abad8d3a6b0a2e31d45a0b78/images%20and%20video/Signs/Proposed%20Signs%201.png" width="700" height="550"></p>
<p align="center">Original Proposed Signs
  
We decided to use Roboflow because it is a very versatile website that allows you to train custom models, source annotated datasets for training, and/or find datasets with models that are already trained. Roboflow is a really great resource for finding and implementing computer vision models on a number of devices which includes the OAK-D camera we have on our car. We learned to make sure to source a model with the model type YOLO v8 when using an OAK-D camera. This ensured that the camera could communicate with the model via the ROS2 package we later installed onto our NVIDIA Jetson Nano. 

As we explored Roboflow, we began to transition the model we proposed since we realized that there are datasets with a large variety of annotated images. Since some of these models had thousands of images with specified classes, we decided that our car may respond better if we used a model that was trained using more data. This transition led us to use a model that trained hand signs instead:

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/6c93144ac21b37f17492fffeda7a3398a52009c6/images%20and%20video/Signs/Transition%20to%20Hand%20Signs.png" width="700" height="600"></p>
<p align="center">Transition to Hand Signs

Model training worked great so we installed a sourced ROS2 package, provided by a github link from our TA, which contained the code we modified for our own applications. We had installed and modified this package a couple of days prior, and were already prepared to present these results during the update presentation on 09/03/2024. In fact, we were already “troubleshooting” the code. It is important to note however, that our code was not producing any errors by 09/02/2024. This leads us to believe that this may have been the point where we should have been able to move forward with programming our vehicle with commands. Unfortunately, we believe that due to trouble with our VESC, an issue we had previously tried to resolve, we were not able to get the car to respond. We spent the next days continuing on our journey of trying to get the car to respond but eventually collaboration with Team 5 led us to install a new package which you see located in the “src” directory. After installing this package, we ran into the same issue with our VESC which hindered us from testing any actual commands with our car. We are confident however, that we had all other components necessary for our car to respond to classes it recognized. Below you can see model training and class recognition in action. Here we tested two different trained models with distinct hand sign classes:


<p align="center"><img src="https://github.com/ncucsd/The-Puppy/tree/1721c2832739c1117f58061601e65e52e94b524c/images%20and%20video/Video%20Demonstrations" ></p>
<p align="center">Please click the link above to access the videos of our trained model demonstrations.


This is the Github link for anyone interested: https://github.com/UCSD-ECEMAE-148/winter-2024-final-project-team-6 



### Goals

- Get the car to follow an individual
- Get the car to respond to commands while following the individual



### Accomplishments

- learned how to train a custom model on Roboflow
- learned how to source a public data set with a trained model on Roboflow
- learned how to install a package using ros2 that uses a model from Roboflow
- The robot is able to recognize specific hand signs as classes from models trained on Roboflow



### CAD Design
<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/1721c2832739c1117f58061601e65e52e94b524c/images%20and%20video/CAD/Board%20Complete.png" ></p>
<p align="center">Board

<p align="center"><img src="https://github.com/ncucsd/The-Puppy/blob/1721c2832739c1117f58061601e65e52e94b524c/images%20and%20video/CAD/Spark%20Switch%20Housing%202.png" ></p>
<p align="center">Antispark Switch Housing

Some parts needed for the initial construction of the robot were designed by a teammate who unfortunately departed from our team. Also some hardware already had cases.



### Acknowledgements:

We want to give a big thank you to our TAs Alexander Haken and Eric Foss as well as Professor Jack Silberman for guiding ua through this journey. Your help and patience will not be forgotten.
