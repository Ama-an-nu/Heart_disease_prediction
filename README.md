# Heart_disease_prediction
Deep learning model for Heart_disease_prediction, learnings through MITOCW

# ❤️ Heart Disease Prediction using Deep Learning

A binary classification project that uses an Artificial Neural Network (ANN) to predict the presence of heart disease based on patient health attributes.

This project was completed as a hands-on learning exercise based on the **MIT OpenCourseWare Deep Learning lecture and original Google Colab notebook**.

## 📌 Project Overview

The objective is to build and train a neural network on tabular patient data and evaluate its ability to classify whether a patient has heart disease.

The project explores the complete deep learning workflow, from data preprocessing and feature engineering to model training and evaluation.

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Google Colab

## 📊 Dataset

The project uses the Heart Disease dataset containing:

- **303 patient records**
- **13 original independent features**
- **1 target variable**

The features include:
- Age
- Sex
- Chest pain type
- Resting blood pressure
- Serum cholesterol
- Fasting blood sugar
- Resting ECG results
- Maximum heart rate
- Exercise-induced angina
- ST depression
- Other clinical attributes

**Target:** Binary classification indicating the presence or absence of heart disease.

Dataset: [Heart Disease Dataset – UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/45/heart+disease)

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Loaded the dataset using Pandas.
- Separated numerical and categorical features.
- Applied One-Hot Encoding to categorical variables.
- Standardized numerical features using training-set mean and standard deviation.
- Split the dataset into 80% training and 20% testing data.
- Converted processed data into NumPy arrays.

### 2. Neural Network Architecture

Implemented a feedforward neural network using TensorFlow and Keras.

| Layer | Configuration |
|---|---|
| Input Layer | 29 features |
| Hidden Layer | Dense layer, 16 neurons |
| Hidden Activation | ReLU |
| Output Layer | Dense layer, 1 neuron |
| Output Activation | Sigmoid |

### 3. Model Compilation

- **Optimizer:** Adam
- **Loss Function:** Binary Crossentropy
- **Evaluation Metric:** Accuracy

### 4. Model Training

| Parameter | Value |
|---|---|
| Epochs | 300 |
| Batch Size | 32 |
| Validation Split | 20% |
| Random Seed | 42 |

The model's training and validation loss and accuracy were monitored across epochs to understand its learning behaviour and identify potential overfitting.

## 📈 Results

The trained neural network achieved the following test performance:

| Metric | Result |
|---|---:|
| Baseline Accuracy | 72.6% |
| Neural Network Test Accuracy | **83.61%** |
| Test Loss | 0.4810 |

The neural network achieved approximately **11 percentage points higher accuracy** than the baseline model.

### Model Evaluation

The model was evaluated using:

```python
model.evaluate(test_X, test_y)
```

Output:

```text
Accuracy: 0.8361
Loss: 0.4810
```

## 🧠 Key Learnings

Through this project, I gained practical experience in:

- Understanding feedforward neural networks.
- Working with numerical and categorical tabular data.
- One-Hot Encoding and feature standardization.
- Building neural network architectures using Keras.
- Understanding ReLU and Sigmoid activation functions.
- Model compilation and optimization using Adam.
- Training models using mini-batches and multiple epochs.
- Monitoring training and validation performance.
- Evaluating a binary classification model.

## 📂 Project Files

```text
Heart-Disease-Prediction/
│
├── Heart-Disease-Prediction.ipynb
├── README.md
└── demo.mp4
```

## 🚀 How to Run

1. Clone this repository:

```bash
git clone <your-repository-url>
```

2. Navigate to the project directory:

```bash
cd Heart-Disease-Prediction
```

3. Install the required libraries:

```bash
pip install tensorflow numpy pandas matplotlib
```

4. Open the notebook using Jupyter Notebook or Google Colab.

5. Run the notebook cells sequentially.

## 📚 Learning Reference

**MIT OpenCourseWare – Deep Learning**

This project follows the original lecture material and Google Colab notebook. The implementation and experimentation were carried out as part of my personal learning journey.

## ⚠️ Disclaimer

This project is intended for educational purposes only. It is not a clinically validated diagnostic system and should not be used for medical decisions.

---

**Learning by building, experimenting, and improving.** 🚀


