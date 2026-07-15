# 🏦 AI Credit Risk & Loan Eligibility Classifier

## 📌 Overview
 
**Loan Eligibility Prediction System** is a full-stack machine learning web application that predicts whether a loan applicant is eligible for approval in real time. It combines a trained **scikit-learn classification model** with a lightweight **Flask** backend and a clean **HTML/CSS** front end, delivering instant, data-driven decisions based on applicant profile data.
 
This project demonstrates an end-to-end ML workflow — from data preprocessing and model training to deployment as an interactive web application.
 
---

 ![](https://github.com/MDAsif-bit01/CRC_ML_PROJECT/blob/main/loan_eligibility_preview.png)
 
## 🚀 Key Features
 
- 🔮 **Real-time prediction** — Instant loan eligibility results served through a simple web form
- 🧠 **Trained ML classifier** — Predicts approval outcomes using applicant financial & demographic data
- ⚖️ **Feature scaling pipeline** — Ensures consistent, normalized inputs for reliable predictions
- 🌐 **Web-based interface** — Accessible via browser, no technical knowledge required to use
- 🔁 **Reusable model artifacts** — Trained model and scaler are serialized (`.pkl`) for fast loading and easy redeployment
- 🎨 **Clean, responsive UI** — Built with custom HTML/CSS for a smooth user experience
---
 
## 🧩 How It Works
 
1. The user enters applicant details into a web form (age, income, loan amount, credit score, employment years, education level, housing status).
2. The Flask backend receives the form data and converts it into a structured numerical array.
3. The data is passed through a pre-fitted **scaler** to normalize the feature values.
4. The scaled data is fed into a **pre-trained classification model**, which outputs a prediction.
5. The result — **"Eligible for Loan ✅"** or **"Not Eligible ❌"** — is rendered back to the user instantly.
---
 
## 🛠️ Tech Stack
 
| Layer                | Technology                   |
|----------------------|------------------------------|
| **Backend**          | Python,                      |
| **Machine Learning**  | scikit-learn, NumPy, Pandas |
| **Frontend**         | HTML5, CSS3                  |
| **Model Artifacts**  | Serialized `.pkl` files (model + scaler) |
 
---
 
## 📥 Input Features
 
| Feature            | Description                                  |
|---------------------|-----------------------------------------------|
| `Age`              | Applicant's age                               |
| `Income`           | Applicant's annual/monthly income             |
| `Loan_Amount`      | Requested loan amount                         |
| `Credit_Score`     | Applicant's credit score                      |
| `Employment_Years` | Years of employment history                   |
| `Education_Level`  | Encoded education level                       |
| `Housing_Status`   | Encoded housing/ownership status              |
 
---
 
## 📂 Project Structure
 
```
CRC_ML_PROJECT/
│
├── app.py                       # Flask application & prediction route
├── index.html                   # Front-end form and results page
├── style.css                    # UI styling
├── loan_model.pkl                # Pre-trained ML classification model
├── scaler.pkl                    # Fitted feature scaler
├── loan_eligibility_preview.png  # App preview screenshot
└── README.md
```
 
---
 
## ⚙️ Installation & Setup
 
```bash
# 1. Clone the repository
git clone https://github.com/MDAsif-bit01/CRC_ML_PROJECT.git
cd CRC_ML_PROJECT
 
# 2. Install dependencies
pip install flask numpy scikit-learn 
 
# 3. Run the application
python app.py
```
 
Then open your browser and go to:
```
http://127.0.0.1:5000/
```
 
---
 
## 🖥️ Usage
 
1. Launch the app using the steps above.
2. Fill in the applicant details in the web form.
3. Click **Predict**.
4. View the instant eligibility result on the same page.
---
 
## 📈 Model Details
 
- **Type:** Supervised machine learning classifier (scikit-learn)
- **Preprocessing:** Feature scaling via a fitted `StandardScaler`/scaler object
- **Serialization:** Model and scaler persisted with `joblib` for fast, consistent inference
- **Output:** Binary classification — *Eligible* vs. *Not Eligible*
 
---
 
## 🔮 Future Improvements
 
- [ ] Add model performance metrics dashboard (accuracy, precision, recall, F1-score)
- [ ] Deploy to a cloud platform (Render, Heroku, AWS, etc.)
- [ ] Add input validation and error handling on the form
- [ ] Expand to a multi-model comparison (Logistic Regression vs. Random Forest vs. XGBoost)
- [ ] Add REST API endpoint for programmatic access
- [ ] Add unit tests for the prediction pipeline
---
 
## 👤 Author
 
**MD Asif**
🔗 [GitHub Profile](https://github.com/MDAsif-bit01)
 
---
 
## 📄 License
 
This project is open source and available under the [MIT License](LICENSE).
 
---
 
⭐ If you found this project useful or interesting, consider giving it a star!
