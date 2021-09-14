Main aim of the project is to identify wires in the construction debris to promote reusing and recycling of construction waste
The project is done by group of 6 people headed by me

We have built ML model from scratch creating own image dataset, training the model, improving the model accuracy

We have tried using simple set of CNNs but that didn't give good results, So we used VGG19 model as feature extractor and added a regressor to it to predict the probability of presence of wire,

Threshhold of 0.8 probability is selected as we want good precision bcz we are using the model to reduce man power in seperating wires from the debris and don't want sorted objects to contain other objects as well

We are able to improve accuracy from 60% to 95% using VGG model

Our model is able to predict the wires if they are present near but unable to detect them if they are far away(as the details will be lost during resizing the image to smaller input size), 
but the robots will be working on nearby objects so it doesn't create much problem

Future plannings:
To create bounding boxes for the wires using computer vision techniques so that it will be easier for the robot to pick the wire
