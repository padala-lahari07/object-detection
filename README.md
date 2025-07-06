# 🎯 Object Detection using MobileNet-SSD

This repository demonstrates **real-time object detection** using the **MobileNet Single Shot Detector (SSD)** model with **OpenCV** and **Python**. The model detects multiple common objects such as people, cars, dogs, phones, and more in images, video files, or live webcam feeds.

---

## 🧠 Model Overview

- **Architecture**: MobileNet + Single Shot Multibox Detector (SSD)
- **Framework**: OpenCV Deep Neural Network (dnn) module
- **Pre-trained on**: Caffe (COCO/ILSVRC datasets)

MobileNet-SSD offers a great balance between speed and accuracy, making it ideal for real-time applications.

---

## 📂 Project Structure

```bash
mobilenetssd-object-detection/
│
├── object_detection_ssd.py             # Main detection script
│
├── models/
│   ├── MobileNetSSD_deploy.caffemodel  # Pre-trained weights
│   └── MobileNetSSD_deploy.prototxt    # Network architecture
│
│
└── README.md                           # Project documentation
```

---

## 🚀 How to Run

### 📦 Step 1: Clone Repository & Install Dependencies

```bash
git clone https://github.com/yourusername/mobilenetssd-object-detection.git
cd mobilenetssd-object-detection
pip install opencv-python
```

### 📁 Step 2: Download Pretrained Model Files

Download the following two files and place them in the `models/` directory:

- [`MobileNetSSD_deploy.prototxt`](https://github.com/chuanqi305/MobileNet-SSD/blob/master/MobileNetSSD_deploy.prototxt)
- [`MobileNetSSD_deploy.caffemodel`](https://github.com/chuanqi305/MobileNet-SSD/blob/master/MobileNetSSD_deploy.caffemodel)

### ▶️ Step 3: Run the Detection Script

#### For image input:
```bash
python object_detection_ssd.py --image test_images/example.jpg
```

#### For webcam:
```bash
python object_detection_ssd.py --webcam
```

#### For video file:
```bash
python object_detection_ssd.py --video test_videos/demo.mp4
```

---

## 📝 Supported Object Classes

The MobileNet-SSD model can detect the following 20 classes:

```
['background', 'aeroplane', 'bicycle', 'bird', 'boat',
 'bottle', 'bus', 'car', 'cat', 'chair',
 'cow', 'diningtable', 'dog', 'horse', 'motorbike',
 'person', 'pottedplant', 'sheep', 'sofa', 'train', 'tvmonitor']
```

---

## 💻 Sample Output

![sample-detection](https://raw.githubusercontent.com/yourusername/mobilenetssd-object-detection/main/sample_output.jpg)  
*Real-time object detection with bounding boxes and class labels*

---

## 🧪 Performance

- **Inference Speed**: ~20-30 FPS on standard laptop CPU (no GPU)
- **Input Size**: 300x300 pixels (resized automatically)
- **Threshold**: Detection confidence ≥ 0.5 (default, configurable)

---

## 📦 Requirements

```bash
python >= 3.6
opencv-python
```

Install via pip:
```bash
pip install opencv-python
```

---

## 📌 References

- MobileNet-SSD (Caffe) implementation by [chuanqi305](https://github.com/chuanqi305/MobileNet-SSD)
- OpenCV DNN documentation: [https://docs.opencv.org/](https://docs.opencv.org/)
- SSD: Single Shot MultiBox Detector Paper: [https://arxiv.org/abs/1512.02325](https://arxiv.org/abs/1512.02325)

---

## 👤 Author

**Padala Lakshmi Sai Lahari**  
B.Tech in CSE (AI) | ML & CV Enthusiast  
🔗 [LinkedIn](https://www.linkedin.com/in/padala-lakshmi-sai-lahari-b08b59259) • 🐙 [GitHub](https://github.com/padala-lahari07)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
