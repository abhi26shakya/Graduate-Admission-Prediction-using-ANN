# 🎓 Graduate Admission Prediction using ANN (Regression Model)

## 📌 Overview

This project predicts the **chance of admission** for students based on academic and profile features using an **Artificial Neural Network (ANN)**.

It is a **regression problem**, where the output is a continuous value (probability of admission between 0 and 1).

---

## 🚀 Features

* Data preprocessing using Pandas & NumPy
* Removal of unnecessary columns
* Feature scaling using MinMaxScaler
* ANN model built using TensorFlow/Keras
* Model evaluation using R² Score
* Visualization of training and validation loss

---

## 🧠 Tech Stack

* Python 🐍
* NumPy
* Pandas
* Scikit-learn
* TensorFlow / Keras
* Matplotlib

---

## 📂 Dataset

* Dataset used: `Admission_Predict.csv`
* Contains features such as:

  * GRE Score
  * TOEFL Score
  * University Rating
  * SOP (Statement of Purpose)
  * LOR (Letter of Recommendation)
  * CGPA
  * Research Experience
* Target:

  * **Chance of Admit (continuous value)**

---

## ⚙️ Project Workflow

### 1️⃣ Data Loading & Cleaning

* Load dataset using Pandas
* Drop unnecessary column (`Serial No.`)

---

### 2️⃣ Feature Selection

* `X` → Input features
* `y` → Target variable (Chance of Admit)

---

### 3️⃣ Train-Test Split

* 80% training data
* 20% testing data

---

### 4️⃣ Feature Scaling

* Apply **MinMaxScaler**
* Scale features to range [0,1]

---

### 5️⃣ Model Architecture

* Input Layer (7 features)
* Hidden Layer (7 neurons, ReLU)
* Hidden Layer (7 neurons, ReLU)
* Output Layer (1 neuron, Linear activation)

---

### 6️⃣ Model Compilation

* Loss Function: `mean_squared_error`
* Optimizer: `Adam`

---

### 7️⃣ Model Training

* Epochs: 250
* Validation Split: 20%

---

### 8️⃣ Evaluation

* Metric: **R² Score**
* Measures how well the model fits the data

---

## 📊 Results

* Model achieves a good **R² score** on test data
* Shows strong predictive performance
* Some **overfitting observed** (training loss lower than validation loss)

---

## 📈 Visualization

* Training vs Validation Loss Graph
* Helps detect:

  * Overfitting
  * Underfitting
 
<img width="585" height="452" alt="loss_vs_epoch_graph" src="https://github.com/user-attachments/assets/5ac574a2-bd3b-4c19-a389-b74d5e23a788" />



---

## 📁 Project Structure

```
├── Admission_Predict.csv
├── ann_regression.ipynb
├── README.md
├── requirements.txt
```

---

## 🛠️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/your-username/admission-prediction-ann.git

# Navigate to project folder
cd admission-prediction-ann

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook
```

---

## 🎯 Future Improvements

* Add EarlyStopping to reduce overfitting
* Use Dropout layers
* Perform hyperparameter tuning
* Compare with Linear Regression, Random Forest
* Deploy model using Streamlit

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repository and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## ⭐ Support

If you found this project useful, give it a ⭐ on GitHub!
