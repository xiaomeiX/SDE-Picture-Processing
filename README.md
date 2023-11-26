# SDE-Picture-Processing
Introduction:
Image Processor application is a cloud-hosted, distributed system. It allows the user to apply transformations on top of image in order. 
Transformations include grayscale, flip horizontally, flip vertically, resize, thumbnail, rotate -/+ n degrees, Black and white, blend image. 
User will upload the image from their hard drive and send requests for transformations along with an image. 
Application on the server side will apply transformations, process the image, and then return the result image. 

Language/Design choices: Python3, Flask and Pillow from python liberary 
1.	API accepts and produces application; charset=UTF-8 content type.
2.	Python as a primary language. Python3 version is used to develop applications.
3.	To create REST APIs and manage applications, Flask is used to implement API.
4.	CORS is enabled for all domains for all paths.
5.	The image is stored on application memory.
6.	Import Pillow from Python library to process image. Pillows as external libraries to process image need be installed before starting the sever.
7.	API works on HTTP protocol. 
8.	The image to be processed is sent to API.
9.	The client must provide at least one transformation, in a valid format, when using API to process image.
10.	The application will validate the user’s input before posting it to the server. 
11.	For the front end, use HTML and CSS to create a dynamic web form by using “POST and GET” to interact with servers. 

CI/CD:
AWS Code Pipeline is used to automate the delivery and deployment process.
