# 🏠 House Price Prediction with MLflow

This project implements a **House Price Prediction model** using the California Housing dataset, with a complete **MLOps workflow** powered by **MLflow**. The notebook demonstrates the end-to-end process of training a machine learning model, performing hyperparameter tuning, logging experiments, and registering the best-performing model.

---

## 📌 Project Overview

The project follows these steps:

1. **Data Preparation**  
   - California Housing dataset is loaded and structured into features (`X`) and target (`y`).  
   - Data split into training and testing sets.  

2. **Model Training**  
   - A **Random Forest Regressor** is used for predicting house prices.  
   - Hyperparameter tuning is performed with **GridSearchCV**.  

3. **Experiment Tracking with MLflow**  
   - Every run logs **hyperparameters**, **metrics** (MSE, R²), and **artifacts**.  
   - Multiple runs are compared in the **MLflow UI**.  
   - The best model is **registered** in the MLflow Model Registry.  

4. **Evaluation**  
   - Model performance is evaluated on test data using Mean Squared Error (MSE) and R² score.  
   - Best performing run is selected for deployment readiness.  

---

## 📂 Repository Structure

-   `housepricepredict.ipynb`: Jupyter Notebook with full workflow
-   `requirements.txt`: Python dependencies

---

## ⚙️ Installation & Setup

Follow these steps to run the project on your local machine:

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/house-price-mlflow.git
cd house-price-mlflow
```

### 2. Create a virtual environment
```bash
python -m venv venv
```
Activate it:
Windows:
```bash
venv\Scripts\activate
```
Mac/Linux:
```bash
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch MLflow UI
```bash
mlflow ui
```

This will start MLflow on `http://127.0.0.1:5000`.

### 5. Run the Jupyter Notebook

Execute all cells in housepricepredict.ipynb to train models, perform hyperparameter tuning, and log results in MLflow.

---

## 📊 MLflow Features in this Project

✅ Experiment Tracking – log all hyperparameters and metrics

✅ Comparison of Runs – analyze performance across experiments in the MLflow UI

✅ Model Registration – register the best-performing Random Forest model

✅ Reproducibility – results can be replicated across environments

---

## 🚀 Future Enhancements

* Add other regression models (XGBoost, LightGBM) for comparison
* Deploy the registered model as a REST API using MLflow
* Containerize the application with Docker for production use

---

## 📝 Author

**👤 Your Name**

* **GitHub:** yourusername
* **LinkedIn:** Your LinkedIn

---

## 📜 License

This project is licensed under the MIT License.
