# brain-tumor-cnn-classification
Brain Tumor Detection and Classification using CNN

## 📌 Project Overview

This project focuses on detecting and classifying brain tumors from MRI images using Convolutional Neural Networks (CNNs).

The model classifies MRI images into four categories:

- Glioma Tumor
- Meningioma Tumor
- No Tumor
- Pituitary Tumor

This project was developed as an academic machine learning project to study image classification using deep learning.

## 📂 Dataset

The project uses the **Brain Tumor MRI Dataset** available on Kaggle.

Dataset source:

https://www.kaggle.com/datasets/bilalakgz/brain-tumor-mri-dataset

The classification dataset contains:

- Training images: 2,870
- Testing images: 394
- Total images: 3,264
- Number of classes: 4

## 🔄 Preprocessing

The following preprocessing steps were applied:

- Images resized to `128 × 128`
- Pixel values normalized to the range `[0, 1]`
- Images loaded using Keras `ImageDataGenerator`
- Categorical labels used for multi-class classification

Data augmentation was also tested using:

- Rotation
- Width and height shifting
- Zooming
- Horizontal flipping

## 🧠 CNN Models

Four CNN approaches were experimented with:

1. **Basic CNN**
2. **CNN + Data Augmentation**
3. **CNN + Batch Normalization**
4. **Deeper CNN**

The models were implemented using TensorFlow and Keras.

## 📊 Results

| Model | Test Accuracy |
|---|---:|
| Basic CNN | 72.08% |
| CNN + Data Augmentation | 41.88% |
| CNN + Batch Normalization | 71.07% |
| Deeper CNN | 56.60% |

The results show that model performance varies depending on the architecture and preprocessing technique.

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- GitHub

## 📁 Project Files

- `*.ipynb` — Complete Google Colab notebook
- `Brain_Tumor_CNN_Project_Report.docx` — Project report
- `results/model_comparison.csv` — Model comparison results

## ▶️ How to Run

1. Download or clone this repository.
2. Open the Jupyter Notebook in Google Colab.
3. Download the dataset from Kaggle.
4. Upload/configure your Kaggle API credentials in Colab.
5. Run the notebook cells sequentially.

## ⚠️ Limitations

The test dataset was also monitored during model training as validation data, so it should not be considered a completely unseen test set.

The reported model results come from separate recorded training runs rather than one synchronized training session.

## ⚕️ Disclaimer

This project is intended for **educational and research purposes only**.

It is not a clinically validated medical diagnostic system and should not be used to make medical decisions.

## 👨‍💻 Project

**Brain Tumor Detection and Classification using CNN**

Developed as an academic deep learning project.
