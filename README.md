# Face-mask-recognition

INTRODUCTION-
Real-Time Face Mask Detector :-During pandemic COVID-19, WHO has made wearing masks compulsory to protect against this deadly virus thus, will build a real-time system to detect whether the person on the webcam is wearing a mask or not. We will train the face mask detector model using Keras and OpenCV and few other libraries.

OBJECTIVE OF PROJECT-
1. As the name indicates this project is about detecting the face mask in Real-Time.
2. The purpose Of project is detect the whether the person is wearing mask or no mask and give warning if the person is not wearing mask as we learnt how important masks cause of corona pandemic.
3. This project can be used for other Purposes too like a simple face detector or a gender detector.

TECHNOLOGIES USED-
1. Python
2. Tensorflow (object detection library) 
3. Keras
4. MobileNet
5. OpenCV

BLOCK DIAGRAM OF MY PROJECT-
![image](https://user-images.githubusercontent.com/76063534/133553861-839757f2-9013-4d6c-9326-9ba480994487.png)

There are two phases in total in our project – 

Phase 1 – Training the model
Phase 2 – Applying the model

METHODOLOGY-
1. To train the Face Mask Detector, user needs the Face Mask Dataset. Bigger dataset (more images) give better predictions. 
2. We’ll focus on loading our face mask detection dataset from disk, training a model using Keras on this dataset, and then serializing the face mask detector to disk.
3. Once the face mask detector is trained, we can then move on to loading the mask detector, performing face detection.
4. Now using OpenCV we can capture the image of the face through webcam.
5. Once the face is detected, extract the face ROI (Region Of Interest) (which can be nose and mouth region) using OpenCV.
6. Now we can apply the face mask classifier (trained model) to detect whether the face in the screenshot has a mask or not.
7. Once detected, the result is outputted.

DATASET-
Download the data set from any decent data set site. I used “https://www.kaggle.com/wobotintelligence/face-mask-detection-dataset”

With Mask--
![image](https://user-images.githubusercontent.com/76063534/133553953-96750a63-3731-482f-9184-7aa2cb0ba64c.png)

Without Mask--
![image](https://user-images.githubusercontent.com/76063534/133554006-fb3d84e4-bb93-4819-bc2b-cd68538d4bc8.png)

DATA PREPROCESSING-
- Convert the data set images and labels into arrays and Loop the data set images in two list i.e, data and labels.
- Using several libraries functions like – Load_img coming from keras.preprocessing.image which loads an image into PIL (Python image library) format, img_to_arr and few other functions.
![image](https://user-images.githubusercontent.com/76063534/133554197-ce685ae4-ff81-44b0-9fcf-4c88e6cafc0b.png)

TRAINING THE MODEL-
![image](https://user-images.githubusercontent.com/76063534/133554264-82ebf133-f1b4-4a8d-af4f-cb0d801d03ad.png)

Use model in Real-Time camera using openCV
![image](https://user-images.githubusercontent.com/76063534/133554353-cf400eca-9b90-445e-807d-efecbcf8d36a.png)

FINAL RESULT-
Running the final python program we made for the video input using openCV.
![image](https://user-images.githubusercontent.com/76063534/133554441-01bda0e4-adec-464e-a353-7b31e70b31c5.png)

FINAL OUTPUT-

Without Face Mask-
![image](https://user-images.githubusercontent.com/76063534/133554489-4b95e31a-d06c-4e09-8a1b-ab8f5078fef8.png)

With Face Mask-
![image](https://user-images.githubusercontent.com/76063534/133554526-310fc074-e1e0-4a25-8bc9-b5105bd72738.png)











