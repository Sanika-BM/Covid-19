# COVID-19 Detection Using Support Vector Machine (SVM)

## 1. Project Overview

This project uses Machine Learning to detect COVID-19 from chest X-ray images using the Support Vector Machine (SVM) algorithm.

The system classifies chest X-ray images into two categories:
- **COVID:** Patient X-ray image with COVID-19.
- **Normal:** Patient X-ray image without COVID-19.

The model is trained using the COVID-19 Radiography Database available on Kaggle.

## 2. Objectives

- To detect COVID-19 using chest X-ray images.
- To implement the Support Vector Machine algorithm.
- To preprocess and classify medical images.
- To evaluate model performance using different metrics.
- To visualize the results using a confusion matrix.

## 3. Dataset

**Dataset Name:** COVID-19 Radiography Database

**Source:** Kaggle

**Dataset Link:** https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database

The dataset contains four categories:
- COVID
- Normal
- Lung Opacity
- Viral Pneumonia

This project uses only COVID and Normal images for binary classification.

## 4. Technologies Used

- **Programming Language:** Python
- **Platform:** Google Colab
- **Machine Learning Algorithm:** Support Vector Machine (SVM)
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, PIL, KaggleHub

## 5. Methodology

The project follows these steps:

1. Download the dataset from Kaggle.
2. Import the required Python libraries.
3. Load COVID and Normal X-ray images.
4. Convert images into grayscale.
5. Resize images to 64 × 64 pixels.
6. Convert images into numerical arrays.
7. Split the dataset into 80% training and 20% testing.
8. Apply feature scaling.
9. Train the SVM classification model.
10. Predict the test images.
11. Evaluate the model performance.

## 6. Algorithm Used

**Support Vector Machine (SVM)**

SVM is a supervised machine learning algorithm used for classification. It identifies the best decision boundary (hyperplane) to separate different classes.

In this project, Linear Support Vector Classification (LinearSVC) is used to classify chest X-ray images into COVID and Normal categories.

## 7. Evaluation Metrics

The model is evaluated using the following metrics:

- **True Positive (TP):** COVID correctly predicted as COVID.
- **True Negative (TN):** Normal correctly predicted as Normal.
- **False Positive (FP):** Normal incorrectly predicted as COVID.
- **False Negative (FN):** COVID incorrectly predicted as Normal.
- **Accuracy:** Overall correct predictions.
- **Precision:** Correct COVID predictions among predicted COVID cases.
- **Recall:** Correctly identified COVID cases among actual COVID cases.
- **F1-Score:** Balance between precision and recall.

A confusion matrix is generated to visualize the classification results.

## 8. Project Structure

```text
COVID-19-Detection-SVM/
│
├── README.md
│
├── covid19_detection.ipynb
│
└── Results/
    └── confusion_matrix.png
```

## 9. How to Run the Project

1. Open Google Colab.
2. Create a new notebook.
3. Copy the project code into the notebook.
4. Install the required libraries.
5. Download the Kaggle dataset using KaggleHub.
6. Execute each code cell step by step.
7. Train the SVM model.
8. View the predictions and evaluation results.

## 10. Expected Output

The project generates:

- COVID and Normal image samples.
- Trained SVM classification model.
- Predicted classification results.
- Confusion matrix visualization.
- Accuracy, Precision, Recall and F1-score.

## 11. Advantages

- Simple and easy-to-implement classification model.
- Uses medical image data for prediction.
- Provides multiple evaluation metrics.
- Visualizes classification performance.

## 12. Future Enhancements

- Include all four dataset categories.
- Improve classification accuracy.
- Compare SVM with Random Forest and CNN.
- Develop a web-based user interface.
- Explore deep learning techniques.

## 13. Conclusion

This project demonstrates the application of Support Vector Machine for COVID-19 detection using chest X-ray images. Image preprocessing, model training, classification and evaluation are performed to understand the effectiveness of machine learning in medical image classification.

**Note:** This project is developed for academic and educational purposes only. It is not intended for real-world medical diagnosis.