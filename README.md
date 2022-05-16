# CNN-ROI-Detector
In this project, I wanted to apply transfear learning, with a pre-trained model YOLOv4, with the goal of performing detection on two Regions: Face and Forehead. I did this to use as a method tecnique for my masters.
The pre-trained Convolutional Neural Network model was created by Alexey Bochkovskiy, et. Al., and was State-of-Art at the time, and can be found at https://github.com/AlexeyAB/darknet.
For this task, I downloaded thermographic images from the public domain http://tdface.ece.tufts.edu/, them I used the labelImg to label the forehead (testa) and face, as shown in the image below.
![image](https://user-images.githubusercontent.com/62029505/168625479-1cce5cc4-0e6b-4612-9f50-929312db82fd.png)

Then, I trained the model in the google colaboratory cloud with my 300 labeled examples, where 0 was the class testa (forehead), and 1 was the class face. The model achieved good results, with a the Intersection over Union (IoU) normalized metric = 70%.

Prediction example:

![image](https://user-images.githubusercontent.com/62029505/168620901-b2c380f7-1774-4fe4-b7b5-c62b4dd9e019.png)

the YOLO_v4_Treinamento_do_detector.ipynb file contains the model and the transfer learning, with the results for my data;
The obj folder contains the labeled images for training;
The valid folder contains the labeled images for validation;
The Yolo_ImagemTermog folder cointains the instructions I followed for this task;
The Label_img-windows_v1.8.1 folder contains the Imager Labeler that I used to label the thermographic dowloaded images.


