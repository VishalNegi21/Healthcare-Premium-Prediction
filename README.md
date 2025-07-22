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

```bash
1️⃣ Clone the Repository
git clone https://github.com/VishalNegi21/Healthcare-Premium-Prediction.git
cd Healthcare-Premium-Prediction

2️⃣ Install Dependencies
Make sure you have Python 3.8+ installed, then run:
pip install -r requirements.txt

3️⃣ Launch the Streamlit App
Run the main script using:
streamlit run main.py

4️⃣ Enter Inputs in the UI
When prompted in the Streamlit form, provide:
- Age
- Number of dependants
- Income (in lakhs)
- Insurance plan (number: 0, 1, or 2)
- Genetic risk (1 = Yes, 0 = No)
- Normalized risk score (e.g., 0.82)
- Gender (Male or Female)
- Region (Southeast, Southwest, Northwest, Northeast)

✨ Based on your age, the app automatically chooses the correct prediction model and displays your predicted premium.






