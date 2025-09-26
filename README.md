# Raisin Classification Model 🧺🍇

This project uses **machine learning** to classify raisin types (`Besni` and `Kecimen`) based on their physical properties. The model was trained using the **Raisin Dataset** and saved as a `.joblib` file for easy reuse.

---

## 📂 Project Structure

```
├── main.py              # Main script to load and test the model
├── raisin_model.joblib  # Saved trained ML model
├── dataset.xlsx         # Raisin dataset (features + labels)
└── README.md            # Project documentation (you are here!)
```

---

## ⚙️ Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/raisin-classifier.git
   cd raisin-classifier
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   Or install them manually:

   ```bash
   pip install pandas scikit-learn joblib
   ```

---

## 🚀 Usage

### Run the script

```bash
python main.py
```

### Load and use the model in Python

```python
import joblib
import pandas as pd

# Load model
model = joblib.load("raisin_model.joblib")

# Example input (feature values)
sample = [[2000, 0.85, 1.1, 0.5, 0.9, 0.95, 0.2]]  

# Predict raisin type
prediction = model.predict(sample)
print("Prediction:", prediction)
```

---

## 📊 Dataset

The dataset contains physical measurements of raisins with two classes:

* **0 → Besni**
* **1 → Kecimen**

Features include:

* Area
* Perimeter
* MajorAxisLength
* MinorAxisLength
* Eccentricity
* ConvexArea
* Extent

---

## 🏆 Model

* Preprocessing: Scaling + Label Encoding
* Algorithm: (e.g., RandomForestClassifier or whichever you used)
* Evaluation Metric: Accuracy

---

## ✨ Future Improvements

* Add more raisin samples to improve accuracy
* Try deep learning models
* Build a web app interface with Flask/Streamlit

---

## 👨‍💻 Author

* **Omotosho Muyiwa Steven**
