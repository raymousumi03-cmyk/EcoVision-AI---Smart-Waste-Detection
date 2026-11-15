<img width="1287" height="652" alt="Screenshot 2026-11-15 202543" src="https://github.com/user-attachments/assets/31d1175b-c30d-4c0a-a559-d03a7d2cb0d0" />

# ♻️ EcoVision AI – Smart Waste Detection

## Project Overview

EcoVision AI is an AI-based Smart Waste Detection System developed using YOLO (You Only Look Once) and Deep Learning.

The project detects and identifies different types of waste objects from images using a trained YOLO object detection model.

The main objective is to support smart waste management and promote environmental cleanliness through automated waste detection.

##  Project Objectives

- Automatically detect waste objects using AI.
- Identify different categories of waste.
- Display detected objects with bounding boxes.
- Show confidence scores for detected objects.
- Support smart and efficient waste management.

##  Waste Categories

The model is trained to detect the following waste categories:

- Glass
- Plastic_Bag
- Paper_Bag
- Garbage_Bag
- Pet_Bottle
- Can

##  Technologies Used

- Python
- Google Colab
- YOLOv8
- Ultralytics
- Deep Learning
- OpenCV
- Gradio
- Roboflow

##  Project Structure

```text
EcoVision-AI/
│
├── EcoVision_AI.ipynb
├── data.yaml
├── README.md

│
├── models/
│   └── best.pt
│

```

##  Model Training

The YOLO object detection model was trained using a waste detection dataset.

The training process includes:

1. Dataset preparation
2. Data preprocessing
3. YOLO model training
4. Model evaluation
5. Waste object detection

##  How to Run the Project

### Step 1: Install required libraries

```bash
pip install ultralytics gradio opencv-python
```

### Step 2: Load the trained model

```python
from ultralytics import YOLO

model = YOLO("best.pt")
```

### Step 3: Perform detection

```python
results = model.predict(
    source="sample.jpg",
    conf=0.25,
    save=True
)
```

## Output

The system identifies waste objects and displays:

- Detected waste class
- Confidence percentage
- Bounding boxes around detected objects
- Detection results

## Future Enhancements

- Real-time waste detection using cameras.
- Video-based waste detection.
- Waste classification and segregation.
- Integration with smart waste management systems.

##  Project Name

EcoVision AI – Smart Waste Detection
