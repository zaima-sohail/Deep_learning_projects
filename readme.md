## In this rep, there are 50+ plus projects of deep learning with complete readme, setup ,libraries and markdown
## Project1:
# Perceptron Trick

Trains a perceptron (line that splits 2 classes) by fixing mistakes, one point at a time.

## Predict
```
z = w·x + b
ŷ = 1 if z ≥ 0 else 0
```

## Update Rule
```
w = w + lr * (y - ŷ) * x
```

## Steps
Random line → pick random point → wrong? nudge weights → repeat → line separates classes.

## Limitation
Only works if data is linearly separable. If not, transform features first (e.g. `x1² + x2²`).

## Project2: 
# Perceptron Problem

Implementation of a Perceptron classifier from scratch, along with a look at its key limitation — it only works when data is **linearly separable**.

## What's Inside
- Perceptron training using the perceptron trick / gradient descent update rule
- Demonstration of the **perceptron problem**: fails on non-linearly separable data (e.g. XOR, circular patterns)
- Fix using feature **transformation** to make data separable

## Update Rule
```
w = w + lr * (y - ŷ) * x
```

## Limitation Solved Here
| Problem | Cause | Fix Used |
|---|---|---|
| Doesn't converge | Data not linearly separable | Transform features (e.g. x1² + x2²) |


## Tech Used
- Python
- NumPy
- Matplotlib (for visualizing decision boundary)

## Key Takeaway
A basic perceptron can only draw a straight line to separate classes. When data isn't linearly separable, transforming the features (or using a multi-layer network) is required.
## project3:
# Customer Churn Prediction

A machine learning project that predicts whether a customer is likely to churn using a neural network built with TensorFlow/Keras.

## Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib

## Dataset

`Churn_Modelling.csv`

## Model

The neural network uses:

* ReLU activation in hidden layers
* Sigmoid activation in the output layer
* Binary cross-entropy loss
* Adam optimizer

## Result

The model is trained to classify customers into:

* `0` — No Churn
* `1` — Churn
## Project4:
# Handwritten Digit Recognition using MNIST

This project uses **TensorFlow/Keras** to build a neural network that recognizes handwritten digits from the **MNIST dataset**.

### Technologies

* Python
* TensorFlow / Keras
* MNIST Dataset

### Model

The model uses:

* `Flatten` layer to convert 28×28 images into 784 values
* `Dense` layers for classification
* `ReLU` activation
* `Softmax` output layer
* `Adam` optimizer
* `Sparse Categorical Crossentropy` loss

### Result

The model is trained to classify handwritten digits from **0 to 9**.

## How to Run

```bash
pip install tensorflow pandas numpy scikit-learn
```
## Project5:
# Graduate Prediction using ANN

This project uses an **Artificial Neural Network (ANN)** to predict graduate outcomes based on input features.

### Technologies

* Python
* TensorFlow / Keras
* Artificial Neural Network

### Model

* Dense layers with **ReLU** activation
* **Adam** optimizer
* Classification output layer
* Accuracy: **~73%**

### Result

The ANN achieved approximately **73% accuracy** on the test data.

## How to Run

```bash
pip install tensorflow pandas numpy scikit-learn
```

Run the notebook or Python file to train and evaluate the model.
## project 6:
# ❤️ Heart Disease Prediction Using ANN

## 📌 Overview

A machine learning project that uses an **Artificial Neural Network (ANN)** to predict heart disease from 13 clinical features.

## 📊 Dataset

* 303 patient records
* 13 input features
* 1 target column
* Missing values handled using median imputation

## 🧠 ANN Model

```text
Input (13)
   ↓
Dense (32, ReLU)
   ↓
Dense (16, ReLU)
   ↓
Output (1, Sigmoid)
```

**Loss:** Binary Crossentropy
**Optimizer:** Adam

## 📈 Result

The model achieved approximately **85% test accuracy**.

## 🛠️ Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow/Keras
* Matplotlib
## Project7:
 # Credit Card Fraud Detection Using Deep Artificial Neural Network

