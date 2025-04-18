# RealTimeSignLanguageDetector
Using python, meadiapipe and opencv we were able to analyse data from the webcam and also identify landmarks on the hand that can be used to create datasets of x and y coordinates. Using these datasets,we trained a random forest classifier using scikit-learn to create a sign language model. Putting it all together, the model can be used in real time in conjuction with opencv to detect hand signs.

Dataset can be downloaded from: https://www.kaggle.com/datasets/ayuraj/asl-dataset

How to try it out

Pull the project/Download a zip and open in an IDE of your choice
Run the files in the order
collect_imgs (Follow the steps on screen to collect images)
create_dataset
train_classifier (This should reveal the classifier score in the console)
test_classifier (Final file that should run the model in real time)We trained it on 100 images for each letter of the alphabet (36 classes for 26 letters+10 for digits). The labeling process for each image ensured that the model could accurately recognize each sign language letter during a video, even with variations in hand shape and movement.
-----> In the real-time detection phase:

Start Webcam Feed: Launch the real-time detection script.
Perform Gestures: Perform the ASL gestures in front of the webcam.
View Predictions: See the predicted gesture and probability visualization on the screen.
The webcam feed is processed frame by frame.
Key points are extracted and fed into the trained model.
The model predicts the gesture being performed.
The predicted gesture is displayed on the screen, along with a visualization of prediction probabilities.Here are few snippets representing real time detection performed

![IMG-20250418-WA0015](https://github.com/user-attachments/assets/45e14891-aadd-4f7c-9001-83142ed2eec4)
![IMG-20250418-WA0018](https://github.com/user-attachments/assets/ed3bd20e-7d64-4c61-89a0-0bad81e0a9a2)
![IMG-20250418-WA0017](https://github.com/user-attachments/assets/73001e9f-a533-4bd4-98d2-a0f4c77a9a7c)
![IMG-20250418-WA0016](https://github.com/user-attachments/assets/7651af63-6150-4f53-9e86-0b58832b6dd1)
![IMG-20250418-WA0019](https://github.com/user-attachments/assets/1f2398d5-c79e-4dc1-a0f0-0c00d06be911)
![IMG-20250418-WA0020](https://github.com/user-attachments/assets/912dc24f-ba95-4376-9cf8-3ce8cb10b3b0)
![IMG-20250418-WA0023](https://github.com/user-attachments/assets/f1c28ee4-8429-4457-8489-56d5a6b4e0f2)
![IMG-20250418-WA0022](https://github.com/user-attachments/assets/23291647-a27d-45f6-9c1e-8595a471a838)
![IMG-20250418-WA0021](https://github.com/user-attachments/assets/04b589ba-4f27-4c92-9010-75e693f9b7be)
![IMG-20250418-WA0024](https://github.com/user-attachments/assets/cd311d9c-77d6-452f-8705-f240a2f6cf46)
![IMG-20250418-WA0025](https://github.com/user-attachments/assets/908a3d39-bd3a-493e-a467-0deff6b754c0)
![IMG-20250418-WA0026](https://github.com/user-attachments/assets/7b501a0a-4d21-4bfe-adb9-224df9cae66a)
![IMG-20250418-WA0028](https://github.com/user-attachments/assets/7e69160d-9f71-48e4-b490-9d9fa63afebd)
![IMG-20250418-WA0005](https://github.com/user-attachments/assets/3be9eb5c-afd8-44ea-9450-e13fe097b2f8)
![IMG-20250418-WA0006](https://github.com/user-attachments/assets/af26d05f-4b0f-49b6-8e88-3d5baf7c611d)
![IMG-20250418-WA0007](https://github.com/user-attachments/assets/beab9711-6793-41be-8d36-89773510c1fa)
![IMG-20250418-WA0010](https://github.com/user-attachments/assets/07fb2a17-83b0-456d-b56c-6efb27ce1315)
![IMG-20250418-WA0009](https://github.com/user-attachments/assets/27a8c9d7-d8e1-4b1f-91c4-22660ff79bf3)
![IMG-20250418-WA0008](https://github.com/user-attachments/assets/d9e984ad-05ce-440a-b13b-201335284ba4)
![IMG-20250418-WA0011](https://github.com/user-attachments/assets/05f4cc0b-f612-43ad-a774-bcf321fa21bd)
![IMG-20250418-WA0013](https://github.com/user-attachments/assets/36addde3-5f04-4ba0-80e3-b35dda2db6a1)
![IMG-20250418-WA0012](https://github.com/user-attachments/assets/e20f4e54-944a-41ae-ad00-aa1cc99af1c3)
![IMG-20250418-WA0014](https://github.com/user-attachments/assets/b3d6dbd6-e531-464b-8aaf-2dd62800fd7e)
![IMG-20250418-WA0029](https://github.com/user-attachments/assets/b2f6e522-1451-44e0-ae3d-9361fd1f3287)


                         
