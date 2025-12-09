# 🏦 Bank Churn Prediction

## 📘 Project Overview
Customer churn (also known as customer attrition) is when clients stop doing business with a company.  
This project aims to **predict whether a bank customer will leave (churn)** based on demographic and account-related data.

We use a **Simple Artificial Neural Network (ANN)** built with **TensorFlow/Keras** to classify customers as “Exited” or “Not Exited.”

---

## 🧠 Model Overview
We use a **Simple ANN (Artificial Neural Network)** architecture:
- Input Layer → features from the dataset  
- Hidden Layers → fully connected layers with ReLU activation  
- Output Layer → single neuron with sigmoid activation (for binary classification)

### **Model Summary**
| Layer Type | Number of Neurons | Activation | Purpose |
|-------------|-------------------|-------------|----------|
| Input Layer | Depends on number of features | - | Input data |
| Hidden Layer 1 | 64 | ReLU | Learn complex patterns |
| Hidden Layer 2 | 32 | ReLU | Deep feature extraction |
| Output Layer | 1 | Sigmoid | Predict churn probability |

---

## 📊 Dataset
The dataset used is **Bank Customers Churn Dataset** (e.g., `Churn_Modelling.csv`).

### **Columns**
| Feature | Description |
|----------|--------------|
| CreditScore | Customer credit score |
| Geography | Country of residence |
| Gender | Male/Female |
| Age | Age of customer |
| Tenure | Years with the bank |
| Balance | Account balance |
| NumOfProducts | Number of bank products used |
| HasCrCard | Whether customer has a credit card |
| IsActiveMember | Whether customer is active |
| EstimatedSalary | Annual salary |
| Exited | Target variable (1 = churned, 0 = stayed) |

---

## ⚙️ Steps Involved

1. **Import Libraries**
   - TensorFlow, Keras, Pandas, NumPy, Matplotlib, Scikit-learn.

2. **Data Preprocessing**
   - Encode categorical variables (LabelEncoder, OneHotEncoder).
   - Split dataset into train and test sets.
   - Standardize features using `StandardScaler`.

3. **Build ANN Model**
   - Sequential model with Dense layers.
   - Activation functions: ReLU and Sigmoid.

4. **Compile Model**
   ```python
   model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])

---

## :sparkles: Streamlit

🔗 Live Demo  
👉 [click here to open the Streamlit App](https://bank-churn-prediction-using-simple-ann.streamlit.app/)
