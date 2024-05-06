# FacialRecognition

![demo of the model using the webcam](assets/demo.gif)

YOLOv5 model trained on custom dataset of 1,187 images containing faces. Interestingly, the model has no problem identifying a face that has an object obscuring the lower part of a face. However, the model struggles to identify the face where the left or right side of the face is obscured. This is likely because the training data contains images of faces that are covered by masks where the bottom of the face is obscured. 

Originally I planned to used the FDDB dataset that contains thousands of more faces. This dataset uses ellipses instead of rectangles to identify faces, so I wrote some code that translate this into rectangular bounding boxes. This dataset was way too large to train on locally so I ended up abandoning it to train on a smaller dataset from RoboFlow.

Training information can be found in the directory "yolov5s_results6". Training this model locally took about 28 hours on M3 Macbook.
