# 🚲 Bike Rental Prediction with Kernel Regression  

## 📌 Project Overview  

This project predicts the **total number of bicycles rented per day (`cnt`)** using a kernel-based regression model.  
It explores how weather conditions, seasonality, and other factors influence daily bike rental demand.  

The workflow covers data cleaning, preprocessing, exploratory analysis, and model building using advanced regression techniques.  

**Authors:** Juliana Bermúdez & Valentina Herrera  
**Course Assignment:** Punto 2  

---

## 📊 Dataset  

The dataset contains daily records of bike rentals along with various explanatory variables.  

**Features used in the model:**  
- `season` – season of the year  
- `mnth` – month  
- `yr` – year indicator  
- `holiday` – whether the day is a holiday  
- `workingday` – whether the day is a working day  
- `weekday` – day of the week  
- `temp` – normalized temperature  
- `windspeed` – wind speed  

**Target variable:**  
- `cnt` – total count of bikes rented  

---

## ⚙️ Project Structure  
```
├── PUNTO2.ipynb # Main Jupyter notebook with full analysis
├── data/ # Dataset files (not included in repo)
├── README.md # Project description (this file)
```

---

## 📝 Methodology  

1. **Data Loading & Preprocessing**  
   - Import required libraries (pandas, numpy, scikit-learn, etc.).  
   - Load the dataset into a Pandas DataFrame.  
   - Drop non-predictive identifiers (`date`, `instant`).  
   - Convert integer-coded categorical variables into proper categories or dummy variables.  
   - Verify absence of missing values.  

2. **Exploratory Data Analysis (EDA)**  
   - Summary statistics of all features.  
   - Visualization of distributions and correlations between variables.  

3. **Modeling**  
   - Build a kernel-based regression model to predict `cnt`.  
   - Split data into training and test sets.  
   - Train and tune the model.  
   - Evaluate performance with metrics such as **R²**, **RMSE**, and **MAE**.  

4. **Results & Insights**  
   - Present model accuracy and error metrics.  
   - Discuss which features most strongly affect bike rental demand.  

---

## 🛠️ Requirements  

Install the dependencies:  

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
