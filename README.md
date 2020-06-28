# Mask-Detection
The given repo mainly shows how to train custom objects on yolov3.

## About YOLO
You only look once (YOLO) is a state-of-the-art, real-time object detection system.The full detail of the working of YOLO and its performance is given in detail in the following link. 

[YOLO](https://pjreddie.com/darknet/yolo/)

## Training Custom objects

Yolov3 is trained on coco dataset but we can train it for our own custom datasets,detailed information is given on the particular github repo

[darknet-custom objects](https://github.com/AlexeyAB/darknet)

Mainly four custom files should be added for detecting the desired objects, as I have done for mask detection.

[obj.data](https://github.com/Sinha199/Mask-Detection/blob/master/obj.data)

[obj.names](https://github.com/Sinha199/Mask-Detection/blob/master/obj.names)

[yolov3_obj.cfg](https://github.com/Sinha199/Mask-Detection/blob/master/yolov3_mask.cfg)

## Important points for training 

As per my model I have trained it till 2000 iterations(total 6000 iterations) that took me nearly 6 hours because of GPU constraints.For efficient training store the last trained model and then ,resume the training from the last pretrained weights.This is the link to the 2000th iterations of the model. This can be used for further efficient training,
[Trained weights](https://drive.google.com/file/d/1vXQR53Bej19MKqHn3MRcem9nJioJws9A/view?usp=sharing)


## Dataset 

This is link to the dataset, [images](https://drive.google.com/drive/folders/1zyihcNoo8A6qugSxGAZOZgpKxZzGvqnx?usp=sharing)

The folder containes the images and the corresponding text files which contain the annotations of the masked and non-masked images. For annotations of images I have used [LabelImg](https://github.com/tzutalin/labelImg) , its a tool graphical image annotation tool.

## Overview of Prediction
[prediction.gif]
