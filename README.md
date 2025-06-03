# 🥑 Avocado Ripeness Prediction

This project predicts avocado ripeness levels using a combination of physical (firmness, weight, size) and visual (hue, saturation, brightness) features. It includes full EDA, model training, interpretability, and business application recommendations.

---

## 📊 Dataset
The dataset includes 250 avocados with the following features:
- Firmness, hue, saturation, brightness
- Sound when tapped (in dB)
- Weight (grams), size (cm³)
- Color category and ripeness level (target)

---

## 🚀 Key Features

- ✅ Exploratory Data Analysis (12-plot dashboard)
- ✅ Feature Engineering (color intensity, density, ratios)
- ✅ Model Training with 6 algorithms + ensemble
- ✅ Cross-validation, hyperparameter tuning
- ✅ Dimensionality reduction (PCA, t-SNE)
- ✅ Permutation feature importance
- ✅ Interactive prediction function
- ✅ Business insights + recommendations

---

## 🧠 Best Model

- **Random Forest Classifier**
- **Accuracy:** 100%
- **Top Features:** firmness, sound_db, hue

---

## 📁 Files Included

| File                                | Description                                   |
|-------------------------------------|-----------------------------------------------|
| `Avocado_Ripeness.ipynb`            | Full notebook with EDA, modeling, evaluation  |
| `avocado_ripeness_model.pkl`        | Trained best model artifacts                  |
| `avocado_ripeness_final_model.pkl`  | Final model after ensemble evaluation         |
| `avocado_ripeness_dataset.csv`      | Raw dataset                                   |
| `/utils/predictor_module.py`        | Clean reusable prediction functions           |

---

## 🔍 Sample Prediction

```python
predict_avocado_ripeness(
  firmness=5.2, hue=120, saturation=80, brightness=60, 
  sound_db=45, weight_g=180, size_cm3=150
)
# ➜ Output: "firm-ripe" (confidence: 0.390)
