
+++ title = "Bowdie " 
summary = "Senior Design project UTA CSE Spring 2020 " 
+++
## Background 
In this Project we aimed to create a Application for the Vuzik's Blade smart glasses. 

## Students
# Sergio Guerrero
# Vivek Patel
# Roshan Shrestha
# Micah Hall
# Connor Morris
## System Overview
Bowdie’s architecture involves two main components: the smartglass application and a server. The smartglass application contains five subsystems that operate directly on the glasses: the Vuzix Blade system, the computer vision system, the AR display system, the map and routing system, and the gesture sensing system. The Vuzix Blade system includes the core functionalities provided by the Vuzix Blade glasses including the built-in microphone, the built-in speech processing capabilities, the Vuzix speech recognition library, and internet search capabilities. The computer vision system includes the built-in camera on the glasses, an API request sender that communicates with the server’s API, an object recognition handler that uses object recognition results, a text recognition handler that uses text recognition results, and a coin counting handler that uses coin counting results. The AR display system includes the physical display in the lens of the glasses and the logic for displaying information from other parts of the application. The map and routing system includes a speech handler that performs custom speech recognition to obtain a destination from the user, the Google Maps Directions API that provides routing information, parsing logic that extracts results from the Google Maps API, and a routing processing algorithm that navigates the user through their route. Lastly, the gesture sensing system includes a hand-held sensor that gathers positional data and a gesture sensing algorithm that detects the gestures the user makes with the sensor. The server includes an API that communicates with the application to perform object recognition, text recognition, coin counting, and speech recognition. For object recognition and text recognition, the server uses an image sent from the application with Bing’s Visual Search API to extract vision information to be displayed in the app. For coin counting, the server uses the image with YOLO, having been trained on images of coins. Finally for speech recognition, the server uses audio recorded by the map and routing system’s speech handler with Google’s Cloud Speech-to Text API.
 
## What I worked on 

I worked on the Custom object recognition part of it where I trained US Coins. The end goal was to be able to take a picture of the coins with the Vuzik's blade glasses and it would be able to return you the total amount of money. The concept is simple enough but since I had no experience with Computer Vision I had to do much research. We settled with using YOLOV3 as our method of training since it has it built into it. To train the Coins, I first had to download about 300~ of images of US coins and use labelImg to label the coins in the images so the model could get to know what each different coin looked like in different settings. For the training I used Google Collab GPU. Once I did the training which took about 10 Hours, I downloaded the weights file to the VM that we were using and began testing with images taken with the Vuzik's blade. I quickly realized that it was not going to work since the images taken by the glasses were a much lower resolution. We took around 300 images with the glasses and once again labeled those and ran the model. We got better results but not perfect. 