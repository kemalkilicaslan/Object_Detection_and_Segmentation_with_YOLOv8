# YOLOv8 Object Detection
## Installation
```
pip install ultralytics
```
___
### Image Detection
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
![img](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Image.jpg)

**Object detection in image**
![detectimg](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Object_Detection_With_YOLOv8/Object_Detection_Image.jpg)
___
### Video Detection
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
[![video](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Video.jpg)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object detection in video**
[![Object_detection_in_video](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Object_Detection_With_YOLOv8/Object_Detection_Video.jpg)](https://www.youtube.com/watch?v=lvPSlkSZqyA)
___
### Live Detection
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

**Object detection with snapshot from camera**
[![Object_detection_with_snapshot_from_camera](https://github.com/kemalkilicaslan/YOLOv8_Vision/blob/main/Object_Detection_With_YOLOv8/Real_Time_Object_Detection_Video.jpg)](https://www.youtube.com/watch?v=yvONGbaFJ0g)
