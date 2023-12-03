# IndonesiaForAI-Project-2-Person-Tracking

# Person Tracking Using Faster RCNN and YOLO
> Using Faster RCNN and YOLO


Dalam deteksi objek khususnya person tracking, terdapat beberapa tantangan dikarenakan perubahan pose dan interaksi antar objek dalam satu frame. 

Eksplorasi algoritma Faster RCNN dan YOLO diharapkan memberikan solusi terkait deteksi manusia yang cepat dan akurat. 

Proyek ini bertujuan mengatasi kendala deteksi dalam kerumunan, perubahan pose, dan pemantauan real-time, mendukung pengembangan sistem pelacakan manusia yang lebih efisien..

![](header.png)

## Installation

Install fiftyone:

```sh
!pip install fiftyone
!pip install fiftyone-db-ubuntu2204
```

Install other dependencies:

```sh
!wget https://raw.githubusercontent.com/pytorch/vision/main/references/detection/transforms.py
!wget https://raw.githubusercontent.com/pytorch/vision/main/references/detection/engine.py
!wget https://raw.githubusercontent.com/pytorch/vision/main/references/detection/utils.py
!wget https://raw.githubusercontent.com/pytorch/vision/main/references/detection/coco_eval.py
!wget https://raw.githubusercontent.com/pytorch/vision/main/references/detection/coco_utils.py
```

## Usage Coco-2017 Dataset

```sh
import fiftyone as fo
import fiftyone.zoo as foz

# Load the COCO-2017 dataset
# This will download it from the FiftyOne Dataset Zoo if necessary
dataset = foz.load_zoo_dataset("coco-2017", split="train", label_types=["detections"], classes=["person"], max_samples=4000)
dataset_test = foz.load_zoo_dataset("coco-2017", split="validation", label_types=["detections"], classes=["person"], max_samples=500)
```

## More informatioan About Development and Evaluation

Pretrain Weight using pytorch.

[https://pytorch.org/vision/main/models.html](https://pytorch.org/vision/main/models.html)

Evaluation For fiftyone Setup.

[https://docs.voxel51.com/tutorials/evaluate_detections.html](https://docs.voxel51.com/tutorials/evaluate_detections.html)

## Faster R-CNN Models

* Backbone
    * GoogLeNet
    * MobileNet
    * ResNet50
  
## Yolo Models

* YOLO V3
    * YOLO V3u
* Yolo V5
    * YOLO V5s
    * YOLO V5x
* Yolo V8
    * YOLOV8m
    * YOLOV8l
    * YOLOV8x

## Contributing

10  awsome people
CV B and CV D

