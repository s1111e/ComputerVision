# ComputerVision


# 🚘 Object Detection & Multi-Object Tracking for Autonomous Driving
A complete pipeline for evaluating how different object detection models impact multi-object tracking performance using the KITTI dataset.

---

## Overview  
This project investigates the relationship between **detection accuracy** and **tracking stability** in autonomous driving.  
Four detection models were fine-tuned on the KITTI Object Detection dataset and evaluated on the KITTI Tracking dataset using two modern trackers.

### **Detection Models**
- YOLO11  
- RetinaNet (ResNet-50-FPN)  
- Faster R-CNN  
- Mask R-CNN (bbox mode)

### **Tracking Algorithms**
- DeepSORT (appearance + Kalman filter)
- ByteTrack (IoU-based association)

### **Main Question**
> **How does the choice of object detector affect multi-object tracking (MOT) performance?**

---

## 📑 Abstract  
This project examines four state-of-the-art detection models and evaluates how their accuracy affects multi-object tracking performance.  
We fine-tune each model on KITTI Detection, then run them on KITTI Tracking sequences with DeepSORT .

Results show that:

- **Fine-tuning significantly improves detection.**
- **Higher detection accuracy → fewer ID switches & smoother tracks.**
- **YOLO11 fine-tuned achieves the highest overall performance.**
