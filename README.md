# Project-Gray-Scale-Image-
Converting Color Image to Gray-Scale Image – Weighted method
In this java project I made an image processing application I used concepts like multiple inheritance , encapsulation , abstraction and polymorphism 
First of all , the project is organized in 2 packages : packWork and packTest (in packTest we have the main). 
By running main , first of all we need to select the path of our image . 
I used multi-threading programming in order to change every pixel from my image : 
-ProducerThread obtains every pixel from the image and sends them to ConsumerThread 
-ConsumerThread (this is the location of the algorithm) \ receives the pixels from ProducerThread 
and modifies them with the weighted method and sends them to WriteResultThread with the help of pipes 
-WriteResultThread receives the modified pixels from ConsumerThread and creates a new image with these pixels . 
A new modified image will be created in the location of the original image .
