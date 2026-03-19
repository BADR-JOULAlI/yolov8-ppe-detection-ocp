# Computer Vision Surveillance: PPE Detection Using YOLOv8

## Description

This project aims to develop an automated system for detecting Personal Protective Equipment (PPE) in an industrial environment using computer vision, specifically the YOLOv8 model (You Only Look Once). The goal is to enhance safety on industrial sites by continuously monitoring the use of safety helmets and vests.

The YOLOv8 model is fine-tuned on a dataset combining open-source sources and collected images, augmented using Roboflow, and optimized on Tesla T4 GPUs.

## Features

* **Real-time detection** of PPE (helmets and vests) on images or video streams.
* **Results visualization** with bounding boxes and labels on detected objects.
* **Alerts for non-compliance**, e.g., absence of helmets or vests.

## Project Objectives

The objective of the project is to create a functional proof of concept that enables continuous monitoring of PPE usage in industrial environments, reducing the risks of accidents due to non-compliance with safety protocols.

## Technologies Used

* **YOLOv8**: Object detection model.
* **PyTorch**: Deep learning framework.
* **Roboflow**: Platform for dataset management and image augmentation.
* **OpenCV**: For video stream handling and displaying detections.
* **Kaggle Notebooks**: For training the model on GPUs.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/username/repository-name.git
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the pre-trained YOLOv8 model and place it in the `models/` directory.

## Usage

To run the real-time detection script using a webcam, use the following command:

```bash
python detect.py --source webcam --weights models/yolov8m.pt --img-size 640
```

This will start a video stream where the model will perform predictions on detected objects (helmets, vests, etc.).

## Results

The model's performance is measured with the following metrics:

* **mAP50**: 0.773
* **mAP50-95**: 0.408
* **Precision**: 0.744
* **Recall**: 0.731
* **F1-Score**: 0.738

## Conclusion

This project demonstrated that using YOLOv8 for PPE detection is feasible in industrial environments. The results show good prediction accuracy, offering a more efficient solution for real-time surveillance.

## Authors

* **JOULALI Badr** (Student)
* **TOUIJRE Mohamed** (Professional Supervisor)


