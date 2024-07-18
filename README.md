# Object Detection of PPE (Personal Protective Equipment)

## Project Overview

This project focuses on developing an object detection system for identifying and classifying various types of Personal Protective Equipment (PPE) in images or video feeds. PPE includes items such as helmets, safety vests, goggles, headcap and earplugs.

## Objectives

1. **Detect PPE Items:** Identify and classify different types of PPE in images.
2. **Ensure Safety Compliance:** Assist in monitoring and ensuring compliance with safety regulations.
3. **Real-Time Detection:** Enable real-time detection and alert systems for use in workplaces.

## Features

- **Model Training:** Training of object detection model using YOLOv8. The model was trained using this [dataset](https://universe.roboflow.com/epp-internship-0rrmj/epp-internship-2-no-negatives). 
- **Object Detection:** Object detection and classification given images and videos.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.9 or higher
- Ultralytics
- PyTorch 
- OpenCV

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/ppe-detection.git
   cd ppe-detection
    ```

2. Python Libraries:

   ```bash
   pip install ultralytics
   pip install opencv-python
    ```

### Installation

#### Object Detection files

To run the object detection model on pre-existing files, use the notebook [safety_detection.ipynb](safety_detection.ipynb)
. It is necessary to place the files inside the folder **files_detection/images** or **files_detection/videos**.

Inside the notebook, it is possible to choose different models to perform the detection:

```python
# Load a model
model = YOLO("model/choose_model.pt") 
````

The models can be found inside the folder **model**.

#### Object Detection Webcam

