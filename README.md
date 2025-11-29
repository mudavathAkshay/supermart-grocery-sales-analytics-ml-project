# Supermart Grocery Sales – Retail Analytics & Machine Learning Project

This repository contains an end-to-end **Data Analytics + Machine Learning** project built using the **Supermart Grocery Sales – Retail Analytics Dataset**.  
The dataset represents fictional grocery order records from customers in **Tamil Nadu, India**.  
The project includes **EDA, feature engineering, visualizations, and an ML model for sales prediction**.

---

## 📌 **Project Overview**

The primary goal of this project is to:

✔ Understand sales patterns across categories, regions, cities, and months  
✔ Perform exploratory data analysis (EDA)  
✔ Visualize trends and insights  
✔ Build a machine learning model to predict **Sales**  
✔ Evaluate model performance using regression metrics

Dataset fields include:

- Order ID  
- Customer Name  
- Category  
- Sub Category  
- City  
- Order Date  
- Region  
- Sales  
- Discount  
- Profit  
- State  
- Month / Year (engineered)

Dataset Source: Provided in PDF :contentReference[oaicite:0]{index=0}  
Download Link: *(from original document)*

---

## 🛠 **Technologies Used**

- **Python**
- **NumPy, Pandas**
- **Matplotlib, Seaborn**
- **Scikit-learn**
- **Jupyter Notebook / Kaggle Environment**

---

## 📂 **Project Structure**

📦 supermart-grocery-sales-analytics-ml-project
│
├── data/
│ └── supermart_grocery_sales.csv
│
├── notebooks/
│ └── supermart_sales_analysis.ipynb
│
├── src/
│ ├── eda.py
│ ├── preprocessing.py
│ ├── model_training.py
│ └── visualization.py
│
├── README.md
└── requirements.txt

markdown
Copy code

---

## 📊 **Exploratory Data Analysis (EDA)**

The project includes the following analysis:

### **1. Sales by Category**
Bar chart showing which category contributes most to total sales.  
(Example from PDF: *Egg, Meat & Fish category has highest share* :contentReference[oaicite:1]{index=1})

### **2. Monthly Sales Trend**
Line chart of monthly performance  
(*Sales increase over months* :contentReference[oaicite:2]{index=2})

### **3. Year-wise Sales Distribution**
Pie chart for yearly sales  
(*2017 & 2018 contribute more than 50%* :contentReference[oaicite:3]{index=3})

### **4. Top 5 Cities by Sales**
Bar chart ranking the highest revenue-generating cities.

### **5. Correlation Heatmap**
To understand relationships between Sales, Profit, Discount, etc.

---

## 🔧 **Data Preprocessing**

- Handled missing values and duplicates  
- Converted `Order Date` from object → datetime  
- Extracted:
  - `Order Day`
  - `Order Month`
  - `Order Year`
  - `month_no`  
- Applied **Label Encoding** for:
  - Category  
  - Sub Category  
  - City  
  - Region  
  - State  
  - Month  

---

## 🤖 **Machine Learning Model**

### **Model Used**
- **Linear Regression** (baseline model)

### **Feature Scaling**
- Applied StandardScaler

### **Model Performance**
Mean Squared Error: 1758.26
R-squared: 0.82

yaml
Copy code
(Source: Training output shown in PDF :contentReference[oaicite:4]{index=4})

This indicates a **good predictive performance** with 82% variance explained.

---

## 📈 **Model Evaluation Visuals**

- Actual vs Predicted Sales plot  
- Residual analysis  
- Trend fitting visualization

---

## 🚀 **How to Run the Project**

### **1. Clone the Repository**
```bash
git clone https://github.com/<your-username>/supermart-grocery-sales-analytics-ml-project.git
cd supermart-grocery-sales-analytics-ml-project
