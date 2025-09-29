# ☕ Coffee Sales Prediction & Analysis

A machine learning project to analyze coffee sales data and predict sales amounts using XGBoost. This project uncovers key sales trends, identifies peak hours, and highlights the most popular coffee products, helping businesses and analysts make data-driven decisions.

---

## 📋 Project Description

This project utilizes transaction data to understand and forecast coffee sales. By analyzing features such as payment type, coffee product, time of purchase, and customer card ID, the model provides actionable insights into sales performance and customer preferences.

---

## 🗂️ Dataset

- **Input File:** `index.csv`
- **Columns:**
  - `date`: Transaction date
  - `datetime`: Exact timestamp of purchase
  - `cash_type`: Payment type (cash or card)
  - `card`: Customer card ID (anonymized)
  - `money`: Amount spent
  - `coffee_name`: Coffee product purchased

---

## 🔄 Project Workflow

### 1. Data Cleaning
- Handle missing values.
- Extract features from `datetime` (hour, day, month, etc.).
- Encode categorical variables using Label Encoding.

### 2. Exploratory Data Analysis (EDA)
- Analyze daily sales trends.
- Identify hourly peak sales.
- Examine product-wise sales revenue and popularity.

### 3. Machine Learning
- **Model:** XGBoost Regressor
- **Features:** Time-based features, product, payment type, card ID
- **Target:** `money` (sales amount)
- **Performance:** Achieved R² Score ≈ 0.99

### 4. Feature Importance
- Discover which features most influence coffee sales (e.g., hour of day, product name).

---

## 📈 Results

- **High Accuracy:**  
  - R² = 0.9952  
  - RMSE = 0.34
- **Insights:**  
  - Peak sales occur at **10:00 AM**
  - **Americano with Milk** and **Latte** are the most popular products

---

## 🖼️ Visualizations

- Daily sales trends over time
- Product revenue distribution
- Product popularity counts
- Hourly sales trends
- Feature importance derived from XGBoost

---

## 🧰 Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

---

## 🚀 How to Run

1. **Clone the repository**
    ```bash
    git clone https://github.com/<your-username>/<repo-name>.git
    cd <repo-name>
    ```
2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```
3. **Place `index.csv` in the root directory**
4. **Run the notebook or Python script** to reproduce results

---

## 🔮 Future Work

- Experiment with additional models (RandomForest, LightGBM)
- Deploy as a dashboard (Streamlit/Flask)
- Add forecasting for future sales

---



---

*Contributions and feedback are welcome. If you find this project helpful, please star ⭐ the repo!*
