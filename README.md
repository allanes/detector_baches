## Introduction

This project helps in obtaining a road-damage detection model for assessing potholes study.

Here you will find how to speciallize YOLOv5 and YOLOv7 object detection algorithms in road damage.

For the final pipeline, the cloud-based solutions where used: [Roboflow](https://roboflow.com/) for dataset storage, pre-processing and augmentations and Google Colab for training.

## Installation

1. Open the terminal in the desired directory and clone this project:
   ```
   git clone https://github.com/allanes/pothole-detector-backend.git
   ```

2. Create a new Python environment. Below are the instructions to create one
using *venv* on Windows:
    ```   
    cd pothole-detector-backend
    python -m venv .venv
    .venv\Scripts\activate
    python -m pip install -U pip
    ``` 

3. To install requirements, copy the following commands to the activated 
environment:
    ```
    pip install -U -r yolov5/requirements.txt
    pip install -U -r yolov7/requirements.txt
    pip install -U -r XmlToTxt/requirements.txt
    ```

## How to use

In `etapa1.ipynb` you will find the pre-processing stage for curating the dataset, either locally or through [Roboflow](https://roboflow.com/).

in `etapa2_google_colab.ipynb` you will find the training pipeline used. This is (Google Colab)[https://colab.research.google.com/] ready-to-use. Alternatively, `etapa2_local.ipynb` can be used to perform local training.

Finally, `etapa2_validacion.ipynb` should be used to validate the generated model and to perform the preparations to use it in the [GUI](https://github.com/allanes/pothole-detector-gui).
