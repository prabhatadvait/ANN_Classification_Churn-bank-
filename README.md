
# 🏦 Bank Customer Churn Prediction using ANN

A deep learning web application that predicts whether a bank customer is likely to churn based on various features. Built with **TensorFlow**, **Keras**, and **Streamlit**, and deployed for real-time predictions.

🔗 **[Try the Live App →](https://churnclassificatonannpk.streamlit.app/)**

---

## 🚀 Project Overview

This project uses an **Artificial Neural Network (ANN)** to classify whether a customer will leave (churn) the bank or not, based on their profile. The model was trained using **TensorFlow/Keras**, and the web interface was created using **Streamlit** for user interaction.

---

## 🧠 Technologies Used

- **Python**
- **TensorFlow & Keras** – for building and training the ANN model
- **Pandas & NumPy** – for data preprocessing
- **scikit-learn** – for encoding and scaling
- **Pickle** – to serialize the model, encoders, and scaler
- **Streamlit** – to create and deploy the web application

---

## 📊 Features

- Predicts churn based on:
  - Credit Score
  - Geography
  - Gender
  - Age
  - Tenure
  - Balance
  - Number of Products
  - Credit Card Ownership
  - Active Membership
  - Estimated Salary
- Encodes and scales inputs using saved preprocessing steps (`.pkl` files)
- Easy-to-use UI built with Streamlit
- Real-time prediction output with confidence

---

## 📦 Project Structure

```bash
├── model.h5                   # Trained ANN model
├── ohe_geo.pkl                # OneHotEncoder for Geography
├── label_encoder_gender.pkl   # LabelEncoder for Gender
├── scaler.pkl                 # StandardScaler for numerical data
├── app.py                     # Streamlit app script
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation
```

---

## 💻 How to Run Locally

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/bank-churn-prediction-ann.git
   cd bank-churn-prediction-ann
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit app**

   ```bash
   streamlit run app.py
   ```

---

## 📈 Model Training

- The ANN model was built using `Sequential` from Keras with:
  - Input layer
  - Two hidden layers with ReLU activation
  - Output layer with Sigmoid activation
- Optimized with `Adam` optimizer and `binary_crossentropy` loss
- Evaluation was done using accuracy and loss metrics

---

## 🧪 Example Prediction

A customer with the following input:

```json
{
  "CreditScore": 600,
  "Geography": "France",
  "Gender": "Male",
  "Age": 23,
  "Tenure": 3,
  "Balance": 60000,
  "NumOfProducts": 2,
  "HasCrCard": 1,
  "IsActiveMember": 1,
  "EstimatedSalary": 50000
}
```

✅ **Prediction**: Not likely to churn.

---

## 📎 Links

- 🔗 **Live App**: [https://churnclassificatonannpk.streamlit.app/](https://churnclassificatonannpk.streamlit.app/)
- 📂 **GitHub Repo**: *link to this repo once uploaded*

---

## 🙋‍♂️ Author

**Prabhat Kumar**  
AI/ML Developer | Data Scientist | Full Stack Engineer  
[Portfolio Website](https://prabhatadvait.github.io/Portfolio_Website/) | [LinkedIn](https://www.linkedin.com/in/prabhat-kumar-1260a5259) | [GitHub](https://github.com/prabhatadvait)

---

## 📜 License

This project is licensed under the MIT License. Feel free to use and adapt it.
