# 🏥 Healthcare Premium Prediction

This project predicts healthcare insurance premiums based on user inputs such as age, income, dependents, and medical risk factors. It uses two trained machine learning models — one for younger users (age ≤ 25) and one for older users (age > 25) — to improve accuracy. This is useful for insurance companies to automate and personalize premium pricing.

---

## 🚀 Features

- ML-based healthcare premium prediction
- Separate models for different age groups:
  - `model_young` for users aged ≤ 25
  - `model_rest` for users aged > 25
- Scalers used to preprocess inputs before prediction
- Easy-to-run script with simple command-line interface
- Organized, modular folder structure

---

## 🧠 Tech Stack

- Python 🐍
- scikit-learn
- XGBoost
- joblib
- NumPy, Pandas

---

## 📁 Project Structure


```bash
Healthcare-Premium-Prediction/
│
├── main.py                     # Streamlit app entry point
├── prediction_helper.py        # Model loading and prediction functions
├── premiums.xlsx               # Raw combined dataset
├── premiums_rest.xlsx          # Dataset for users above 25
├── premiums_young_with_gr.xlsx # Dataset for users 25 and below
├── requirements.txt            # Project dependencies
├── README.md                   # Documentation
├── LICENSE                     # License info
└── .gitignore                  # Ignored files and folders
```



---

## 🧪 How to Use

 1. Clone the Repository

```bash
git clone https://github.com/VishalNegi21/Healthcare-Premium-Prediction.git
cd Healthcare-Premium-Prediction
2. Install Dependencies
Make sure you have Python 3.8+ installed. Then run:

bash
Copy
Edit
pip install -r requirements.txt
3. Run the Prediction Script
Navigate to the app/ directory and run:

bash
Copy
Edit
python main.py
4. Enter the Required Inputs
When prompted, enter the following details:

Age

Number of dependants

Income (in lakhs)

Insurance plan (as number: e.g., 0, 1, 2)

Genetic risk (1 = Yes, 0 = No)

Normalized risk score (e.g., 0.82)

Gender (e.g., Male or Female)

Region (e.g., Southeast, Southwest, Northwest, Northeast)

The script will automatically:

Determine which model to use based on the age

Preprocess inputs using the correct scaler

Display the predicted healthcare premium




