# Real-Time Object Detection using YOLOv5  

## Description  
This project implements **real-time object detection** using **YOLOv5 (You Only Look Once version 5)**. The model detects multiple objects in an image or video stream with high accuracy and speed.  

The project was developed as part of an **AI/ML internship**, where the goal was to build an efficient **real-time detection system** using deep learning techniques.  

## Features  
- **Real-time object detection** from webcam or video feed.  
- **YOLOv5 pre-trained models** for high-speed, accurate detection.  
- **Supports multiple classes** (e.g., persons, vehicles, animals, objects).  
- **Integration with OpenCV** for video processing.  
- **Custom dataset training (optional)** for specific object detection.  

## Installation  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/your-username/real-time-object-detection.git
cd real-time-object-detection
```

### 2️⃣ Install Dependencies  
Make sure Python is installed, then install the required libraries:  
```sh
pip install torch torchvision opencv-python numpy matplotlib
```

### 3️⃣ Download YOLOv5  
```sh
git clone https://github.com/ultralytics/yolov5
cd yolov5
pip install -r requirements.txt
```

## Usage  

### **Run Object Detection on an Image**
```sh
python detect.py --source image.jpg --weights yolov5s.pt --conf 0.5
```

### **Run Real-Time Detection via Webcam**
```sh
python detect.py --source 0 --weights yolov5s.pt --conf 0.5
```
*(0 represents the default webcam, change to video path for custom input.)*

### **Train a Custom Model (Optional)**
If you want to train YOLOv5 on a custom dataset:  
```sh
python train.py --img 640 --batch 16 --epochs 50 --data custom_data.yaml --weights yolov5s.pt
```

## Results  
- The model can detect and classify objects in real-time.  
- Performance depends on the **hardware (GPU recommended)**.  
- Custom datasets can improve detection for specific use cases.  

## External Resources & References  
- **YOLOv5 GitHub Repository:** [Ultralytics YOLOv5](https://github.com/ultralytics/yolov5)  
- **YOLOv5 Documentation:** [Ultralytics Docs](https://docs.ultralytics.com/)  
- **Understanding Object Detection:** [Towards Data Science Article](https://towardsdatascience.com/yolo-you-only-look-once-object-detection-explained-492dc9230006)  
- **PyTorch Installation Guide:** [PyTorch Official Site](https://pytorch.org/get-started/locally/)  
- **OpenCV Python Tutorials:** [OpenCV Docs](https://docs.opencv.org/)  

## Dependencies  
- Python 3.x  
- OpenCV  
- PyTorch  
- YOLOv5  
- NumPy  

## Author  
- **Soham Lamb**    
- **GitHub:** https://github.com/SohamAI99  
  
