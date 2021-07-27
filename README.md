# Computer-Vision-AI-Social-Distance-Prediction
COVID-19 outbreak has created a lot of tension and misery to many families across the globe. During this pandemic, people are adviced to not be in close contact with others to reduce the spread of the disease. But there are still many humans who are negligent about this disease by not maintaining social distance. So, I developed this project to monitor if people are maintaining social distance or not. This can help the Government monitor areas where social distancing is not practiced and enforce stricter laws.

Webcam is used to capture the video and detect people in real-time. Using centroid predicted the distances between peoples. If people are very close to each other, a red bounding box is displayed around them indicating that they are not maintainting social distance and for all bounding boxes predicted the distance drawn line printed the distances on that line.


![image](https://user-images.githubusercontent.com/50142455/127100918-08977e92-b224-4fc4-b79c-518695361b61.png)

![image](https://user-images.githubusercontent.com/50142455/127100990-e599a5ee-6e92-4d79-ab02-5a5f265b88cb.png)



# Method
Single Shot object Detection (SSD) using MobileNet and OpenCV were used to detect people. A bounding box is displayed around every person detected.

We have the x, y and z (distance of the person from camera) coordinates for every person in cms. The Euclidean distance between every person detected is calculated using the (x, y, z) cordinates. If the distance between two people is less than 2 metres or 200 centimetres, a red bounding box is displayed around them indicating that they are not maintaining social distance. 
