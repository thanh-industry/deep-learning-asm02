# 🚗 Vehicle Detection using Deep Learning

## 📌 Overview

This project implements and compares two object detection models:

* **YOLOv8 (one-stage detector)**
* **Faster R-CNN (two-stage detector)**

The goal is to detect vehicles (car, bus, motorbike, bicycle) using the **Pascal VOC 2007 dataset**.

---

## 📂 Project Structure

```
01-yolo-v8/
    yolov8_update.ipynb
    yolov8_update_result.ipynb

02-faster-rcnn/
    faster_rcnn.ipynb
    faster_rcnn_result.ipynb

03-report/
    Presentation.pdf

04-demo/
    gradio_image_gui.ipynb
    gradio_video_gui.ipynb
    model_yolov8.pt
    model_fasterrcnn.pt
    Video_Demo.mp4
```

---

## 📊 Results

| Model        | mAP@0.5 | mAP@0.5:0.95 | FPS  |
| ------------ | ------- | ------------ | ---- |
| YOLOv8       | 0.7748  | 0.5568       | 8.07 |
| Faster R-CNN | 0.8623  | 0.5862       | 7.93 |

---

## 🧠 Analysis

* Faster R-CNN achieves **higher accuracy (mAP)**
* YOLOv8 achieves **higher inference speed (FPS)**
* This demonstrates the trade-off between **accuracy and speed**

👉 Faster R-CNN:

* More accurate
* Slower

👉 YOLOv8:

* Faster
* Suitable for real-time applications

---

## 🎮 Demo

### 🖼 Image Demo

Run:

```
04-demo/gradio_image_gui.ipynb
```

Features:

* Upload image
* Compare YOLOv8 vs Faster R-CNN
* Visualize results side-by-side

---

### 🎥 Video Demo

Run:

```
04-demo/gradio_video_gui.ipynb
```

Features:

* Upload video
* Run detection with YOLOv8 or Faster R-CNN
* Export processed video

---

## 📦 Model & Video Files

* Models (`.pt`) and video are stored using **Git LFS**
* This ensures efficient handling of large files

---

## ⚙️ Setup

Install dependencies:

```
pip install torch torchvision ultralytics opencv-python gradio pillow
```

---

## 🚀 How to Run

### Run in Colab

* Open notebook in `04-demo/`
* Run all cells
* Use Gradio GUI

---

### Run locally

```
pip install -r requirements.txt
python gradio_image_gui.ipynb
```

---

## 🎯 Conclusion

* YOLOv8 is suitable for **real-time systems**
* Faster R-CNN is suitable for **high-accuracy tasks**
* Model choice depends on application requirements

---

## 👥 Authors

* Your Name
* Team members

---

## 📚 References

* YOLOv8 – Ultralytics
* Faster R-CNN – PyTorch
* Pascal VOC Dataset
