# YOLOv5 Custom Object Detection
`YOLOv5` (You Only Look Once version 5) is a popular real-time object detection algorithm that uses deep learning techniques to detect and classify objects in images and videos. YOLOv5 was released in 2020 and is the latest version of the YOLO algorithm. YOLOv5 achieves high accuracy and speed by using a smaller network architecture and implementing various optimization techniques, such as focal loss and data augmentation. One of the major advantages of YOLOv5 is its ability to be customized for specific object detection tasks. With YOLOv5, users can train their own custom object detection models using their own dataset of images and labels, making it a versatile solution for various object detection tasks.

# Before You Start
Clone repo and install requirements.txt in a Python>=3.7.0 environment, including PyTorch>=1.7. Models and datasets download automatically from the latest YOLOv5 release.

**Clone GitHub [repository](https://github.com/ultralytics/yolov5)**
```
!git clone https://github.com/ultralytics/yolov5  # clone
```
**install [dependencies](https://github.com/ultralytics/yolov5/blob/master/requirements.txt)**

```Python
%cd yolov5
%pip install -qr requirements.txt  # install
```
**check PyTorch and GPU**

```Python
import torch
import utils
display = utils.notebook_init()  # checks
```
# Testing requirements with pretrained model

`detect.py` runs YOLOv5 inference on a variety of sources, downloading models automatically from the [latest YOLOv5 release](https://github.com/ultralytics/yolov5/releases), and saving results to `runs/detect`. Example inference sources are:

```shell
python detect.py --source 0  # webcam
                          img.jpg  # image 
                          vid.mp4  # video
                          screen  # screenshot
                          path/  # directory
                         'path/*.jpg'  # glob
                         'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                         'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
```
