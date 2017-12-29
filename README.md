## An Intelligence Device Used to Detect and Autofocus 3D Microstructures from Ordinary Optical Microscope

By using three stepper motors to control X-Y-Z position knobs and one servo motor to control the focusing knob, all motors connected to their equivalent Arduinos using PWM digital output and Arduinos connected to NVIDIA Jetson TX2 using a Serial USB cable. From starting point (X0, Y0, Z0) and ending point (Xn, Yn, Zn) on the microscope slide the sample finding mechanism is continuous in a given Z direction where there will be an increment in X till it reaches Xn Then Y after Y increased in one value X starts from X0 to Xn when Y reach Yn Z will increase by one value . A Python script backend with Computer Vision and Machine Learning will see each pixel and control the move of the motors and to find any samples in detected XY area if the sample is matched with our sample it will proceed to the next step else it will continue the process till the ending point (Xn, Yn, Zn) of the microscope slide.


### The AI algorithm 

From finding the microstructures , matching the sample from microscope slide to plotting the equivalent 3D model we use AI. The whole programming language is written using Python. OpenCV, Tensorflow, Keras, Scikit and MatPlot Lib are widely used libraries. We have different scripts for different use. In this paper we will discuss depending on their features. Under training phase, we need to collect dataset and and labeling them then train our model. The second one is using our trained models to find the detect sample. The third one is matching the sample. The forth one is detect and separate the edges to make the 3D Model. All phases and their sub parts are discussed below. 


