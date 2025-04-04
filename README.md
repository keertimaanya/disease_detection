# Potato Disease Detection using Deep Learning

This project focuses on detecting **potato leaf diseases** using a **Convolutional Neural Network (CNN)**. The trained model can classify images of potato leaves into **Healthy, Early Blight, and Late Blight** categories. The model is executed in a Python script, and predictions are displayed in the code editor itself.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Creating a Virtual Environment](#creating-a-virtual-environment)
- [Dataset Preparation](#dataset-preparation)
- [Model Performance](#model-performance)
- [Running the Model](#running-the-model)
- [Usage](#usage)
- [Key Features](#key-features)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)

---

## Project Overview
This project leverages **Deep Learning** to classify potato leaf diseases, assisting farmers in detecting issues early and improving crop health.

### Features:
- **Detects diseases** using a trained CNN model.
- **Provides insights** into classification accuracy.
- **Runs directly in a Python script** without a frontend.

---

## Dataset
- **Source**: Public dataset (PlantVillage)
- **Number of Images**: 5,000+
- **Classes**:
  - `Healthy` → No disease
  - `Early Blight` → Early-stage disease
  - `Late Blight` → Severe infection
- **Structure:**
```
project-directory/
│── dataset/
│   ├── healthy/
│   ├── early_blight/
│   ├── late_blight/
│── model.py
│── README.md
│── potato_disease_model.h5
```

---

## Tech Stack
- **Programming Language**: Python
- **Libraries**:
  - **TensorFlow/Keras** → Model training
  - **Matplotlib/Seaborn** → Data visualization

---

## Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/potato-disease-detection.git
cd potato-disease-detection
```

### Step 2: Creating a Virtual Environment
#### Windows:
```bash
python -m venv env
env\Scripts\activate
```
#### Mac/Linux:
```bash
python3 -m venv env
source env/bin/activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

---

## Dataset Preparation
1. **Download Dataset**: [Potato Leaf Dataset](https://drive.google.com/drive/folders/1tsHzhE6b3byruZ5mv75J-i-Nbb2DK3bT)
2. **Extract Data** into the `dataset/` folder.

---

## Model Performance
- **Accuracy**: ~92%
- **Loss**: ~0.15
- **Confusion Matrix, Precision, Recall** used for performance evaluation.

---

## Running the Model
To test the trained model on an image and get predictions directly in the Python script:

### Step 1: Train the Model
Run the Jupyter Notebook:
```
jupyter notebook trainingpotato.ipynb
```

### Step 2: Modify the Test Image Path
Inside trainingpotato.ipynb, update the test image path:
```
test_image = "path/to/your/test_image.jpg"  # Replace with actual image path
```

### Step 3:  View Predictions
Once the notebook is executed, the model will output a prediction like:
```
Predicted: Early Blight with 89.5% confidence
```

---

## Usage

### Running the Project Locally
1. **Run the Python script**:
```bash
python trainingpotato.ipynb
```
2. **Modify the test image path** inside `trainingpotato.ipynb` to test different images.
3. **View results directly in the terminal.**

---

## Key Features
- **CNN-based disease detection** for potato leaves.
- **Runs without a frontend**, making it simple to use.
- **High accuracy (92%)** trained with TensorFlow.


---

## Conclusion
This project provides a **machine learning solution** for detecting potato leaf diseases. The **CNN model achieves 92% accuracy** and can be easily used in practical applications.

---
