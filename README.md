---

```markdown
# 🧠 Brain Tumor Detector

A deep learning-based project that uses Convolutional Neural Networks (CNN) to classify brain MRI images as **tumor** or **no tumor**. This project aims to support medical professionals by providing an assistive diagnostic tool to improve accuracy and speed of brain tumor detection.

## 📁 Project Structure

```

Brain-Tumor-Detector/
├── Brain Tumor Detector.ipynb
├── README.md
├── dataset/                   # Folder containing MRI images (Tumor / No Tumor)
├── outputs/                   # Model predictions, graphs, results
└── requirements.txt           # Python dependencies

```

## 🧠 Features

- Binary image classification (Tumor vs No Tumor)
- Uses CNN architecture with Keras/TensorFlow backend
- Real-time model evaluation using accuracy and loss plots
- EarlyStopping and ModelCheckpoint used for optimization
- Data preprocessing, augmentation, and training included

## 🖼️ Sample Predictions

<img src="https://via.placeholder.com/300x200?text=Tumor+Detected" width="300"/>
<img src="https://via.placeholder.com/300x200?text=No+Tumor" width="300"/>

## 📌 Dataset

The dataset should contain MRI images organized in two folders:
- `yes/` for tumor images
- `no/` for non-tumor images

You can download a sample dataset from [Kaggle](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection/).

## 🚀 How to Run

### 1. Clone the repository

```

git clone [https://github.com/Jenifa5804/Naan-Mudhalvan-Project.git]
cd brain-tumor-detector

```

### 2. Install dependencies

```

pip install -r requirements.txt

```

### 3. Run the notebook

Open `Brain Tumor Detector.ipynb` in Jupyter Notebook or JupyterLab and run all the cells.

## ⚙️ Model Architecture

* Conv2D → MaxPooling  
* Dropout layers for regularization  
* Flatten → Dense → Output (sigmoid)

```

Input (128x128x3) → Conv2D → MaxPool → Dropout → Conv2D → MaxPool → Flatten → Dense → Sigmoid

```

## 📊 Evaluation Metrics

* Accuracy  
* Loss  
* Confusion Matrix  
* Classification Report

## 📈 Training Performance

* ~95% accuracy on validation set  
* Optimized using Adam optimizer and binary cross-entropy loss  
* Trained for 20 epochs with early stopping

## 📌 Future Enhancements

* Multi-class classification for different types of tumors  
* Integration with Flask or Streamlit for a web-based interface  
* Mobile deployment using TensorFlow Lite  
* Grad-CAM visualization for explainable AI
