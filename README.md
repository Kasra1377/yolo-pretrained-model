### ⭕Object Detection Project With YOLOv3 Model
---
![alt text](image_outputs/cat-dog.jpg)

### 📄Description
---
In this project, our purpose is to use the YOLOv3 pre-trained model for detecting pre-specified objects in images/videos.YOLO algorithms are `single-stage detectors`. As its name suggests, this type of algorithm detects objects without extracting `region proposals` by another model and performing classification tasks on every region. Therefore, this algorithm has a high speed in terms of detecting objects and it can be easily used for real-time object detection tasks. Unlike two-stage detector algorithms, such as `R-CNNs`, `Fast R-CNNs`, and `Faster R-CNNs`, YOLO algorithms are not that accurate. In other words, there is a trade-off between `speed` and `accuracy` in object detection algorithms.

Unlike most object detection algorithms, YOLO variants do not localize the object(s) in the image/video. Instead, these algorithms split the input image into the `SxS` grid. In each grid, we have `m` number of bounding boxes and each bounding box returns a class probability and offset values (offset values are defined for bounding boxes to fit the object more accurately). The bounding boxes that have a value higher than the threshold value are kept to locate the object in the image. The below image shows the process of YOLO algorithms briefly.

![alt text](https://pyimagesearch.com/wp-content/uploads/2018/11/yolo_design.jpg)

[Image Source](https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/)

### 🛠Installation & Configuration
---
In this specific project, the third version of the YOLO algorithm was used. This version has higher mAP on the COCO dataset and higher speed among other versions. In addition to that, YOLO was already trained on the COCO dataset, so no training is required! 
To use the YOLO for object detection, you need three components:
* coco.names
* yolov3.cfg
* yolov3.weights

the first two are available in the `yolo-coco` folder, and you can access the last one via this [link](https://pjreddie.com/darknet/yolo/).
The picture below shows the YOLOv3 performance in terms of other object detection algorithms.
![alt text](https://pjreddie.com/media/image/map50blue.png)

### Results
---
![alt text](image_outputs/soccer.jpg)
![alt text](image_outputs/pedesterians.jpg)

### ❌Limitations
---
YOLO models have some limitations and drawbacks. As mentioned one of them is their accuracy. YOLO models have less accuracy than two-staged models in such a way that they may detect some objects that have weak class probabilities. i.e. this model may detect an SUV as a truck or a train as a bus. Small objects (especially if they are present as a group in an image) may cause a problem for YOLOs in such a way that the YOLO may not even detect them as objects. Because of that, we may have lots of false negatives in some situations.

## 🛠Requirements
---
![](https://forthebadge.com/images/badges/made-with-python.svg)

| Module/Framework        | Version           |
| ----------------------- |:-----------------:|
| numpy                   | 1.19.5            |
| cv2                     | 4.1.2             |
| imutils                 | 0.5.4             |

### ❌Bugs & Issues
---
If you ever encounter bugs in this project or technical issues, you can report them to the `issues` section of this repository, or you can contact me by my email address. 

### 👥Contributers
---
Kasra1377 
