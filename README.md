🏥 Intelligent Healthcare System for Skin Cancer Diagnosis

📌 Project Overview

Skin diseases, especially melanoma, are among the most common health issues worldwide. Early detection is crucial for improving patient survival rates. This project leverages deep learning techniques, particularly CNN architectures, to develop an automated, accurate, and fast diagnostic tool for detecting and classifying skin lesions.

🚀 Features

✔️ Skin lesion segmentation using U-Net

✔️ Classification of lesions with Xception CNN model

✔️ Data preprocessing with augmentation & resizing

✔️ Trained on ISIC 2019 dataset (25,000+ images)

✔️ Implemented with TensorFlow, Keras, OpenCV, and NumPy

📂 Dataset

We used the ISIC 2019 dataset, which includes images from:

    HAM10000 (10,000 images, 600x450 px)
    BCN 20000 (19,424 images, 1024x1024 px)
    MSK dataset

🛑 Data Challenges & Solutions

✅ Class imbalance → Solved with data augmentation
✅ Multiple image resolutions → Addressed with cropping strategies
✅ Missing metadata → Preprocessed accordingly
🏗️ System Architecture

The project follows a two-step process:

1️⃣ Segmentation → Using U-Net to detect and extract lesion areas.
2️⃣ Classification → Applying a fine-tuned Xception model for skin lesion classification into 9 categories.

🔹 Pre-trained Xception model on ImageNet (feature extraction).
🔹 Custom Dense Layer + Softmax activation for classification.
📦 Installation
🔧 Prerequisites

Ensure you have the following installed:

    Python 3.8+
    TensorFlow & Keras
    OpenCV, NumPy, Pandas
    Matplotlib & Seaborn

⚙️ Setup

# Clone the repository
git clone https://github.com/SimedNaiym/skin-cancer-diagnosis.git
cd skin-cancer-diagnosis

# Install dependencies
pip install -r requirements.txt

# Run the model training
python train.py

📊 Results & Performance

✔️ Segmentation Model (U-Net) → Achieves high accuracy in lesion extraction
✔️ Classification Model (Xception) → Fine-tuned for optimal precision & recall
✔️ Evaluated using cross-validation & confusion matrix analysis
