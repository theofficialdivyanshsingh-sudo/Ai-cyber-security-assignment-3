# AI in Cybersecurity – Lab Assignment 3

## Neural Network-Based Cyber Activity Classification

This repository contains my Lab Assignment 3 for AI in Cybersecurity. The project focuses on understanding neural network concepts and implementing a Dense Neural Network to classify cyber activities as **Normal** or **Attack**.

## 📌 Project Overview

The objective of this assignment is to build and evaluate a neural network model for basic cyber activity classification using Python and TensorFlow.

The notebook covers data preprocessing, feature scaling, neural network training, model evaluation, new predictions, and comparison with a Decision Tree classifier.

## 🎯 Objectives

- Understand CNN, RNN/LSTM, GAN and Dense Neural Network concepts.
- Prepare and preprocess a cybersecurity dataset.
- Split data into training and testing sets.
- Apply feature normalization using StandardScaler.
- Build and train a Dense Neural Network.
- Visualize training and validation accuracy and loss.
- Predict whether new cyber activities are Normal or Attack.
- Compare Neural Network and Decision Tree performance.

## 🛠️ Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- TensorFlow / Keras
- Scikit-learn

## 📂 Dataset Information

The project uses a cybersecurity activity dataset containing 100 records.

**Input Features:**
- `failed_logins` – Number of failed login attempts.
- `login_hour` – Hour at which login activity occurs.
- `new_device` – Indicates whether a new device is detected.
- `data_transfer_mb` – Amount of data transferred in MB.

**Target Variable:**
- `0` – Normal Activity
- `1` – Attack Activity

The `record_id` column is excluded from model training because it is an identifier.

## 🧠 Model Architecture

A Dense Neural Network with the following architecture is implemented:

**4 → 8 → 4 → 1**

| Layer | Configuration |
|---|---|
| Input Layer | 4 Features |
| Hidden Layer 1 | 8 Neurons (ReLU) |
| Hidden Layer 2 | 4 Neurons (ReLU) |
| Output Layer | 1 Neuron (Sigmoid) |

**Training Configuration:**
- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Evaluation Metric: Accuracy
- Epochs: 20
- Batch Size: 8
- Validation Split: 20%

## ⚙️ Implementation Workflow

1. Import required Python libraries.
2. Upload and load the cybersecurity CSV dataset.
3. Select input features and target labels.
4. Split the dataset into 75% training and 25% testing data.
5. Normalize features using StandardScaler.
6. Build and train the Dense Neural Network.
7. Plot training and validation accuracy and loss.
8. Evaluate the model using test data.
9. Predict classifications for three new cyber activity records.
10. Compare Neural Network results with a Decision Tree classifier.

## 📊 Model Evaluation

The assignment evaluates model performance using:

- Training Accuracy
- Validation Accuracy
- Testing Accuracy
- Training and Validation Loss
- Classification Report
- Confusion Matrix
- Decision Tree Accuracy Comparison

Actual evaluation results are available in the Jupyter Notebook after execution.

## 🚀 How to Run

**Option 1: Google Colab**

1. Download the `.ipynb` notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the notebook.
4. Run all cells sequentially.
5. Upload the required `simple_cyber_activity.csv` dataset when prompted.
6. Review the generated outputs, graphs, and predictions.

**Option 2: Jupyter Notebook**

1. Clone this repository.
2. Install the required dependencies.
3. Open the notebook in Jupyter.
4. Run the cells in order and provide the dataset when prompted.

## 📁 Repository Structure

```text
AI-in-Cybersecurity-Lab-Assignment-3/
│
├── Lab_assignment_3_Ritik_Sharma_2401010058.ipynb
├── simple_cyber_activity.csv
└── README.md
```

## 📌 Learning Outcomes

Through this assignment, I gained practical experience in:

- Understanding different neural network architectures.
- Applying machine learning preprocessing techniques.
- Developing neural network models using TensorFlow.
- Evaluating classification models.
- Understanding the importance of model interpretability.
- Comparing deep learning models with traditional machine learning algorithms.

## 👨‍💻 Author

**Ritik Sharma**

B.Tech – Computer Science and Engineering

AI in Cybersecurity – Lab Assignment 3

---

