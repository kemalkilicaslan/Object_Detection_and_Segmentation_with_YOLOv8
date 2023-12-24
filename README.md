# Object Detection and Segmentation with YOLOv8

## Installation
```
pip install ultralytics
```
### Object Detection in Photo
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source="img.jpg" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**
![img](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Image.jpg)

**Object Detection in Photo**
![Object_Detection_in_Photo](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Detection_with_YOLOv8/Object_Detection_Image.jpg)
___
### Object Segmentation in Photo
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='img.jpg' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**
![img](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Image.jpg)

**Object Segmentation in Photo**
![Object_Segmentation_in_Photo](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Segmentation_with_YOLOv8/Object_Segmentation_Image.jpg)
___
### Object Detection in Video
#### CLI (Comman Line Interface)
```
yolo detect predict model=yolov8x.pt source="video.mp4" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Video.jpg)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object Detection in Video**
[![Object_Detection_in_Video](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Detection_with_YOLOv8/Object_Detection_Video.jpg)](https://www.youtube.com/watch?v=lvPSlkSZqyA)
___
### Object Segmentation in Video
#### CLI (Comman Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='video.mp4' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Video.jpg)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object Segmentation in Video**
[![Object_Segmentation_inVideo](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Segmentation_with_YOLOv8/Object_Segmentation_Video.jpg)](https://www.youtube.com/watch?v=psdXMi5fQ8U)
___
### Real Time Object Detection
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source=0 show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Detection**
[![Real_Time_Object_Detection](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Detection_with_YOLOv8/Real_Time_Object_Detection_Video.jpg)](https://www.youtube.com/watch?v=yvONGbaFJ0g)
___
### Real Time Object Segmentation
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='0' show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Segmentation**
[![Real_Time_Object_Segmentation](https://github.com/kemalkilicaslan/Object_Detection_and_Segmentation_with_YOLOv8/blob/main/Object_Segmentation_with_YOLOv8/Real_Time_Object_Segmentation_Video.jpg)](https://www.youtube.com/watch?v=bhdDW9Fkcw0)