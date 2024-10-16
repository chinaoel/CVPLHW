
# **CV Homework 1: Object Detection**

The project aims to perform object detection using **DETR** (Detection Transformer), a transformer-based model.

---

## **1. Environment Details**  
Ensure your environment matches the following setup for smooth execution:

- **Python Version:** 3.11.5  
- **CUDA (Optional):** If using GPU, ensure you have the appropriate CUDA drivers installed.  

You can create a virtual environment (recommended) and install dependencies as described below.

---

## **2. How to Run the Code**

### **Step 1: Clone the Repository**
```bash
git clone <your-repo-url>
cd <your-project-folder>
```

### **Step 2: Install Dependencies**
(Optional) Activate your virtual environment
Then, install the required packages:
```
pip install -r requirements.txt
```

### **Step 3: Prepare the Dataset**
Ensure that your dataset is placed in the data/ folder, following the structure below:

```
.
├── data
│   ├── annotations/              # Dataset annotations (COCO-style or JSON)
│   ├── test/                      # Test set
│   │   └── images/                # Test images folder
│   │       ├── img1.png
│   │       ├── img2.png
│   ├── train/                     # Training set
│   │   ├── images/                # Training images folder
│   │   │   ├── img1.png
│   │   │   └── img2.png
│   │   └── labels/                # Training labels folder
│   │       ├── img1.txt
│   │       └── img2.txt
│   └── valid/                     # Validation set
│       ├── images/                # Validation images folder
│       │   ├── img1.png
│       │   └── img2.png
│       └── labels/                # Validation labels folder
│           ├── img1.txt
│           └── img2.txt
├── eval_1009.py                   # Evaluation script
├── lightning_logs/                # Logs from model training
├── requirements.txt               # Dependencies
└── train_huggingface_detr_on_custom_dataset.ipynb  # Training notebook
```

### **Step 4: Run the Jupyter Notebook**
Launch the Jupyter Notebook server and open the training notebook:
Load the DETR model.
Load and preprocess your dataset.
Finetune the DETR model.
Inference and Evaluate on Validation Set and output a json file.
Inference on Testing Set and output a json file.
Visualize the result
