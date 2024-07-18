# Object Detection of PPE (Personal Protective Equipment)

## Project Overview

This project focuses on developing an object detection system for identifying and classifying various types of Personal Protective Equipment (PPE) in images or video feeds. PPE includes items such as helmets, safety vests, goggles, headcap and earplugs.

## Objectives

1. **Detect PPE Items:** Identify and classify different types of PPE in images.
2. **Ensure Safety Compliance:** Assist in monitoring and ensuring compliance with safety regulations.
3. **Real-Time Detection:** Enable real-time detection and alert systems for use in workplaces.

## Features

- **Model Training:** Training of object detection model using YOLOv8. The models were trained using this [dataset](https://universe.roboflow.com/epp-internship-0rrmj/epp-internship-2-no-negatives) and another dataset that is too big to store on Roboflow.
- **Object Detection:** Object detection and classification given images and videos.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following software installed on your machine:

- [Anaconda](https://www.anaconda.com/products/distribution#download-section) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

The languange and libraries utilized will be:

- Python 3.9 or higher
- Ultralytics
- PyTorch 
- OpenCV

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mariamaOlive/internship-ediss.git

   cd internship-ediss
    ```

2. Create a Conda Environment:

    Create a new conda environment using the `environment.yml` file provided in the repository:

   ```bash
   conda env create -f environment.yml
    ```

    Alternatively, you can create your own environment and install the required packages manually:

    ```bash
    conda create --name internship-ediss python=3.9
    conda activate internship-ediss
    conda install jupyter notebook
    pip install ultralytics opencv-python
    ```

3. Activate the Conda Environment:

   ```bash
   conda activate internship-ediss
    ```

4. Launch Jupyter Notebook
    Start Jupyter Notebook:
    ```bash
   jupyter notebook
    ```

    This will open the Jupyter Notebook interface where you can run the notebooks available in this project.

5. Alternative Option to open notebooks:

    - Another option is to run the notebook using Visual Studio Code, and choose the conda environment created as the kernel. *Tip: VS Code is more flexible!*


## Running the Notebooks 📙

1. Navigate through the Jupyter Notebook interface to find the notebook you want to run (files with the .ipynb extension).
2. Click on the notebook to open it.
3. Run the notebook cells by selecting a cell and clicking the "Run" button or pressing Shift + Enter.

## About the Notebooks

### Object Detection files V1
This file perform objet detection on image and video files.

To run the object detection model on pre-existing files, use the notebook [ppe_detection_files_v1](ppe_detection_files_v1). It is necessary to place the files inside the folder `files_detection/images` or `files_detection/videos`.


### Object Detection files V2
This file perform objet detection on image and video files.

To run the object detection model on pre-existing files, use the notebook [ppe_detection_files_v2](ppe_detection_files_v2). 

### Object Detection Webcam
This file perform objet detection using webcam.

To run the object detection model using, use the notebook [ppe_detection_webcam](ppe_detection_webcam). 

### Changing the models

Inside the notebooks, it is possible to choose different models to perform the detection:

```python
# Load a model
model = YOLO("model/choose_model.pt") 
````

The models can be found inside the folder `model`.


