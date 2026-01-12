## 🧠 Real-Time Object Detection with YOLO and OpenCV

This project is a simple implementation of real-time object detection using **YOLO (You Only Look Once)** with **OpenCV** in Python. It allows detection of objects from a webcam feed using either `yolov3` or the lightweight `yolov3-tiny` configuration.

### 🚀 Features

* 🎥 **Real-time Detection:** Detects objects instantly via webcam feed.
* ⚡ **Model Support:** Supports both standard **YOLOv3** (high accuracy) and **YOLOv3-tiny** (faster, for low-end devices).
* 🛠️ **Minimal Setup:** Easy to run with standard Python libraries.
* 📦 **COCO Dataset:** Capable of detecting 80+ object categories out of the box.

### 🗂️ Project Structure

```
├── coco.names               # COCO object class names
├── real_time_yolo.py        # Main script for real-time detection
├── requirements.txt         # Python dependencies
├── yolov3.cfg               # YOLOv3 configuration
├── yolov3-tiny.cfg          # YOLOv3-tiny configuration
└── README.md
```

### 📦 Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/sistem_analiz2_vize.git
   cd sistem_analiz2_vize
   ```

2. Install required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the required weight files:

   * [YOLOv3 weights](https://pjreddie.com/media/files/yolov3.weights)
   * [YOLOv3-tiny weights](https://github.com/smarthomefans/darknet-test/blob/master/yolov3-tiny.weights)

   Place them in the root project folder.

### ▶️ Usage

Run the script with the desired configuration:

```bash
# For full YOLOv3
python real_time_yolo.py --weights yolov3.weights --config yolov3.cfg

# For YOLOv3-tiny (faster, less accurate)
python real_time_yolo.py --weights yolov3-tiny.weights --config yolov3-tiny.cfg
```

### 📌 Notes

* Make sure your webcam is properly connected.
* Accuracy and performance may vary depending on the hardware (GPU recommended for full YOLOv3).
* To stop the detection, press q.
---

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
Copyright (c) 2023 YusufTufan
