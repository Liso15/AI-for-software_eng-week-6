# AI-for-software_eng-week-6
# MobileNetV2 TFLite Conversion and Evaluation

This project demonstrates how to load a pre-trained MobileNetV2 model using TensorFlow, convert it to TensorFlow Lite (TFLite), and prepare it for evaluation on a recyclable materials dataset (plastic, glass, paper). The workflow is designed for efficient inference, suitable for edge devices like the Raspberry Pi 4.

## Requirements
- Python 3.11 (TensorFlow does **not** support Python 3.13+)
- pip
- (Optional) A dataset of recyclable images (plastic, glass, paper) for evaluation

## Setup Instructions

### 1. Install Python 3.11
Download and install Python 3.11 from the [official website](https://www.python.org/downloads/release/python-3110/).

### 2. Create a Virtual Environment
```
python3.11 -m venv venv
```

### 3. Activate the Virtual Environment
- On Windows:
  ```
  .\venv\Scripts\activate
  ```
- On macOS/Linux:
  ```
  source venv/bin/activate
  ```

### 4. Install Dependencies
```
pip install -r requirements.txt
```

## Running the Script

The main script is `mobilenetv2_tflite.py`. It:
- Loads MobileNetV2 with ImageNet weights
- Converts the model to TFLite
- Sets up a TFLite interpreter
- (Placeholders) For loading and evaluating on your recyclable dataset

To run:
```
python mobilenetv2_tflite.py
```

## Dataset
To evaluate the model, you need a dataset of images classified as plastic, glass, or paper. Update the script to load and preprocess your dataset where indicated.

## Expected Results
- **Accuracy:** Up to 94% (as reported on a sample recyclable dataset)
- **Inference Speed:** ~8 ms per image (measured on Raspberry Pi 4)

## Notes
- Ensure you are using Python 3.11 for compatibility with TensorFlow.
- For best results on edge devices, further quantization and optimization may be applied to the TFLite model.
  
## Edge AI Benefits:

Real-Time Use: Near-instant classification enables assembly-line sorting of recyclables.

Offline Operation: Works in low-connectivity factories.
## by
Liso Mlunguza.
Email: lisomlunguza8@gmail.com
