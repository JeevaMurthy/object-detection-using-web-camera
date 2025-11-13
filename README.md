# Object Detection Using Web Camera (YOLOv4 + OpenCV)

This project performs **real-time object detection** using a web camera and the **YOLOv4** deep-learning model. It captures live video frames from your webcam, processes them through the YOLO network, and displays detected objects with bounding boxes and confidence scores—all in real time.

## About the Project
This project demonstrates how modern deep-learning models can identify multiple objects in live video streams with high accuracy and speed. YOLOv4 (You Only Look Once) is a state-of-the-art model known for real-time performance. The system uses:

- `yolov4.weights` — Pre-trained weights  
- `yolov4.cfg` — YOLOv4 model configuration  
- `coco.names` — COCO dataset labels (80 classes)

The program loads YOLO, reads webcam frames, performs detection, applies Non-Max Suppression (NMS), and displays results instantly.

##  Technologies Used
- **Python**
- **OpenCV (cv2 dnn module)**
- **NumPy**
- **YOLOv4**
- **COCO Dataset**

##  Project Structure
```
Object-Detection-Using-Web-Camera/
│── yolov4.cfg
│── yolov4.weights
│── coco.names
│── object_detection.py
│── object_detection.png
└── README.md
```

## ▶️ How It Works
1. Capture webcam frame  
2. Convert to YOLO input blob  
3. Perform forward pass on YOLOv4  
4. Extract boxes, scores, and labels  
5. Apply NMS to remove duplicates  
6. Display bounding boxes and labels  

## 🚀 How to Run
### 1. Install Dependencies
```bash
pip install opencv-python numpy matplotlib
```
### 2. Add YOLOv4 Files

Place these in the same folder:

yolov4.weights

yolov4.cfg

coco.names

### 3. Run the Script
python object_detection.py


Press Q to exit the video window.


### YOLO Detection Flow
Webcam → Preprocessing → YOLOv4 → Predictions → NMS → Output Frame
