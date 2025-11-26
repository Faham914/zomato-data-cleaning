# 🍽️ Zomato Restaurants Dataset — Strict Data Cleaning Project  
### A complete end-to-end data cleaning pipeline by **DataForge Analytics**

This project demonstrates a **professional, strict data-cleaning workflow** performed on a real-world restaurant dataset covering **13 major metropolitan cities in India**.  
The pipeline includes raw data processing, cleaning, outlier removal, preprocessing, documentation, and export of analysis-ready data.

---

## 🚀 Project Highlights

- ✔️ Cleaned 12 attributes across restaurant, cuisine, ratings, items, prices & location  
- ✔️ Applied strict missing value handling  
- ✔️ Standardized all categorical and text features  
- ✔️ Converted numeric columns to proper formats  
- ✔️ Performed **IQR-based outlier detection & removal**  
- ✔️ Generated an automated **cleaning report (JSON)**  
- ✔️ Delivered a clean **final dataset** ready for EDA/ML  
- ✔️ Includes a **Google Colab notebook** and portfolio-ready visuals

---

## 📁 Repository Structure

```
zomato-data-cleaning/
│
├── raw_data/
│   └── zomato_dataset.csv
│
├── processed_data/
│   ├── cleaned_zomato_dataset.csv
│   ├── cleaning_report.json
│   └── portfolio_before_after.png
│
├── notebooks/
│   └── cleaning_script.ipynb
│
└── README.md
```

---

## 🧹 Strict Data Cleaning Pipeline

### **1️⃣ Standardization**
- Uniform column names  
- Trimmed whitespaces  
- Normalized inconsistent text fields  
- Cleaned `best_seller` labels (converted to `bestseller`, `must_try`)

---

### **2️⃣ Duplicate Handling**
- Removed exact and partial duplicate rows  
- Ensured clean row count before/after cleaning  

---

### **3️⃣ Numeric Conversion**
Converted these fields using safe coercion:

- `dining_rating`  
- `delivery_rating`  
- `dining_votes`  
- `delivery_votes`  
- `votes`  
- `prices`  

Invalid values → converted to `NaN` → filled with median (strict policy)

---

### **4️⃣ Missing Values (Strict Removal + Imputation)**

Removed rows missing **critical business fields**:
- restaurant_name  
- item_name  
- cuisine  
- city  

Filled numeric missing values with column medians.

---

### **5️⃣ Outlier Detection & Removal (IQR Method)**

Outliers detected & removed across all numeric fields:

- dining votes  
- delivery votes  
- prices  
- ratings  
- total votes  

Used the industry-standard **1.5 * IQR rule**.

---

### **6️⃣ Categorical Standardization**

- Cleaned and formatted city names to title case  
- Standardized place names  
- Normalized cuisine strings  

---

## 📊 Portfolio Visualization

### **Before vs After (Missing Values Heatmap)**
This visual shows how the dataset improved after cleaning:

`processed_data/portfolio_before_after.png`

---

## 📑 Cleaning Report (JSON)

A machine-readable summary of all actions:

```
original_shape
cleaned_shape
missing_values_after_cleaning
columns
```

Great for clients, employers, and reproducibility.

---

## 🧪 Tools & Technologies Used

- **Python 3**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Google Colab**
- **JSON export**

---

## 🔧 How to Reproduce This Project

1. Open the `cleaning_script.ipynb` notebook  
2. Run the entire pipeline step by step  
3. Upload your dataset when prompted  
4. Export cleaned data & report  
5. Optional: generate portfolio visuals  

---

## 👨‍💼 Author  
### **DataForge Analytics**  
_Data Cleaning • Data Preparation • Dataset Engineering_  
Transforming raw data into analysis-ready gold.

---

## ⭐ If you found this useful  
Give the repo a ⭐ and follow for more pro-level data projects!
