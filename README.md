# 🏡 House Price Prediction - Neural Network Model

## 📌 Project Overview
This project focuses on building a **Neural Network Model** using **PyTorch** to predict **house prices** based on key property features. We started from **raw data**, performed **feature engineering**, **data preprocessing**, **model training**, and **evaluation** using **RMSE (Root Mean Squared Error)**.

## 📊 Dataset Used
- The dataset contains various features related to house attributes such as **square footage, number of rooms, garage size, year built, and neighborhood**.
- The target variable (`SalePrice`) represents the **actual selling price** of the houses.

## 🛠️ Steps Completed
### ✅ 1. **Data Preprocessing**
- Selected the **most relevant features** for price prediction.
- Added a **new feature**: `TotalSF` (Total Square Footage), calculated as:  

- **One-hot encoded categorical variables** (`Neighborhood`, `KitchenQual`).
- **Standardized** all numerical features using `StandardScaler()` to improve model performance.
- **Split** dataset into **training (80%)** and **validation (20%)**.

### ✅ 2. **Neural Network Model in PyTorch**
- Built a **Multi-Layer Perceptron (MLP)** with:
- `Batch Normalization` for stable training.
- `ReLU Activation` for non-linearity.
- `Dropout Layers` to prevent overfitting.
- `Adam Optimizer` for efficient weight updates.
- Defined **Loss Function (`MSELoss`)** for regression.

### ✅ 3. **Model Training**
- Implemented **Early Stopping** to **prevent overfitting**.
- Used **ReduceLROnPlateau** to **dynamically adjust learning rate**.
- **Trained the model** for **up to 100 epochs**, stopping early when validation loss stopped improving.

### ✅ 4. **Evaluation & RMSE Calculation**
- **Converted predictions back to the original price scale** using `StandardScaler.inverse_transform()`.
- **Computed RMSE (Root Mean Squared Error)** to measure model accuracy.

### ✅ 5. **Model Improvement & Testing**
- Compared **RMSE before and after adding `TotalSF`**.
- Adjusted **learning rate, dropout, and batch size** to optimize model performance.

## 📉 Final Results
- **Final RMSE:** _(To be filled in based on your final results)_
- **Lower RMSE → Better price prediction accuracy!** 🎯

## 🚀 How to Run the Model
1. Ensure you have **Python, PyTorch, pandas, and scikit-learn** installed.
2. Load the dataset (`train.csv`, `test.csv`).
3. Run `preprocessing.py` to prepare the data.
4. Train the model using `train.py`.
5. Evaluate predictions and check the RMSE.

## 🔥 Key Takeaways
✅ **Feature Engineering matters** – Adding `TotalSF` improved predictions.  
✅ **Neural Networks work for regression**, but **tuning is key**.  
✅ **Early Stopping & LR Scheduling** help prevent **overfitting**.  

---

### **🎯 Next Steps**
- **Try different architectures (more layers, neurons).**
- **Test on new datasets and check generalization.**
- **Deploy the model for real-time predictions!**

---

🔗 **Author:** _(Your Name)_  
📅 **Date:** _(Today's Date)_  
🚀 **Project Goal:** **Accurately predict house prices using deep learning!**
