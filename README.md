# FacialRecognition

![demo of the model using the webcam](assets/demo.gif)

YOLOv5 model trained on custom dataset of 1,187 images containing faces. Interestingly, the model has no problem identifying a face that has an object obscuring the lower part of a face. However, the model struggles to identify the face where the left or right side of the face is obscured. This is likely because the training data contains images of faces that are covered by masks where the bottom of the face is obscured. 

Training information can be found in the directory "yolov5s_results6". Training this model locally took about 28 hours on M3 Macbook.
