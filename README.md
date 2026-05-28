# Predictive Maintenance with Machine Learning

## 📖 Overview
This project predicts machine failures using sensor data (temperature, speed, torque, wear). Anticipating failures reduces downtime and improves efficiency.

## 📂 Dataset
We use the **AI4I 2020 Predictive Maintenance Dataset** with features like Air temperature [K], Process temperature [K], Rotational speed [rpm], Torque [Nm], Tool wear [min], and a binary target for machine failure.

## ⚙️ Workflow
1. **Preprocessing** → load dataset, clean data, split into features/target.  
2. **Exploratory Analysis** → failure rate, correlations, feature distributions.  
3. **Train/Test Split** → 80/20 split with reproducibility.  
4. **Model Training** → Random Forest Classifier, accuracy evaluation.  
5. **Feature Importance** → identify strongest predictors (Tool wear, Torque).  
6. **Deployment** → Gradio UI for interactive predictions, optional Flask/FastAPI backend.

## 📊 Example Input
```json
{
  "Air temperature [K]": 298.2,
  "Process temperature [K]": 308.7,
  "Rotational speed [rpm]": 1408,
  "Torque [Nm]": 46.3,
  "Tool wear [min]": 3
}
