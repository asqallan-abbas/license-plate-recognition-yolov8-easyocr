# 🚗 License Plate Recognition using YOLOv8 and EasyOCR

This project is part of an internship assignment for **Soulpage IT Solutions**.  
It performs automatic License Plate Detection using YOLOv8 and extracts plate numbers using EasyOCR.

---

## 🔍 Objective

- Detect license plates from vehicle images using YOLOv8 object detection.
- Recognize alphanumeric text on plates using EasyOCR.
- Generate predictions for a test set and export results in CSV.

---

## 📁 Dataset Overview

| Dataset       | Description                                              |
|---------------|----------------------------------------------------------|
| TrainSet1     | 900 vehicle images with bounding box annotations (CSV)   |
| TrainSet2     | 900 cropped plate images with ground-truth text (CSV)    |
| TestSet       | 201 vehicle images used for final testing                |

---

## ⚙️ Project Workflow

1. **Data Loading & Preprocessing**  
   Load training CSV files, unzip images, visualize data samples.

2. **YOLOv8 Annotation Formatting**  
   Convert bounding boxes to YOLO format and save `.txt` label files.

3. **YOLOv8 Model Training**  
   Train a `yolov8n.pt` model with 20 epochs on labeled plate data.

4. **License Plate Detection on Test Images**  
   Detect plates using the trained model.

5. **Text Recognition using EasyOCR**  
   Use EasyOCR to extract license numbers from detected plates.

6. **Exporting Predictions**  
   Save predictions as `final_predictions.csv` with columns:
   `image_name, predicted_plate_number`.

---

## 📦 Files Included

| File Name                    | Description                                      |
|-----------------------------|--------------------------------------------------|
| `License_Plate_Recognition.ipynb` | Full Jupyter Notebook (YOLOv8 + EasyOCR)        |
| `final_predictions.csv`     | OCR output for all 201 test images               |
| `data/*.csv`                | Training annotation files (optional upload)      |
| `images/`                   | Sample input/output images (optional upload)     |

---

## 🛠 Tech Stack

- **YOLOv8 (Ultralytics)**
- **EasyOCR**
- **OpenCV, Pandas, Matplotlib**
- **Google Colab (for training & testing)**

---

---

## 📬 Contact

**Asqallan Abbas**  
[asqallanabbas@gmail.com](mailto:asqallanabbas@gmail.com)

---

