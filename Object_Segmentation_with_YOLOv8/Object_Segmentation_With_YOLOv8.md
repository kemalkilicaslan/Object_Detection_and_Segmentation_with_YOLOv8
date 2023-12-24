# YOLOv8 Object Segmentation
## Installation
```
pip install ultralytics
```
___
### Image Segmentation
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
![img](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Image.jpg)

**Object segmentation in image**
![Object_segmentation_in_image](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Instance_Segmentation_With_YOLOv8/Instance_Segmentation_Image.jpg)
___
### Video Segmentation
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
[![video](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Video.jpg)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object segmentation in video**
[![Object_segmentation_in_video](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Instance_Segmentation_With_YOLOv8/Instance_Segmentation_Video.jpg)](https://youtu.be/psdXMi5fQ8U)
___
### Live Segmentation
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

**Instance segmentation with snapshot from camera**
[![Instance_segmentation_with_snapshot_from_camera](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Instance_Segmentation_With_YOLOv8/Real_Time_Instance_Segmentation_Video.jpg)](https://youtu.be/bhdDW9Fkcw0)
