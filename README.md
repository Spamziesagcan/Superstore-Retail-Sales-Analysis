# 📊 Superstore Sales Analysis - Exploratory Data Analysis (EDA)

## 📈 Project Overview
This project explores the **Superstore Sales Dataset** using **Exploratory Data Analysis (EDA)** techniques. The goal is to uncover insights into **sales trends, profitability, discounts, shipping modes, and regional performance** using data visualization and statistical analysis.

## 🔍 Objectives
- Identify **top-performing categories, sub-categories, and regions**.
- Analyze **sales, profit, and discount distribution**.
- Discover **correlations** between key variables (e.g., sales vs. profit, discount impact).
- Visualize trends using **Seaborn and Matplotlib**.

## 📚 Dataset Information
The dataset includes **retail sales transactions** from a fictional superstore. Key columns include:

| Column Name   | Description |
|--------------|-------------|
| Order Date   | Date of order placement |
| Sales        | Revenue from the sale ($) |
| Profit       | Profit earned per sale ($) |
| Quantity     | Number of items sold |
| Discount     | Discount applied (%) |
| Category     | Product category (Furniture, Office Supplies, Technology) |
| Sub-Category | Detailed product category |
| Ship Mode    | Shipping method used |
| Region       | Geographic region |

## 🛠️ Installation & Setup
1. **Clone this repository:**  
   ```bash
   git clone https://github.com/your-username/superstore-sales-eda.git
   cd superstore-sales-eda
   ```
2. **Install dependencies:**  
   ```bash
   pip install pandas numpy seaborn matplotlib notebook
   ```
3. **Run the Jupyter Notebook:**  
   ```bash
   jupyter notebook Superstore_Retail_Sales_Analysis.ipynb
   ```

## 🎨 Visualizations & Insights
### ✨ Example Plots
#### 1. Sales Distribution
```python
sns.kdeplot(df["Sales"], fill=True, color="blue")
plt.title("Sales Distribution")
plt.show()
```
#### 2. Profit vs. Sales (Bivariate KDE)
```python
sns.kdeplot(data=df, x="Sales", y="Profit", cmap="coolwarm", fill=True)
plt.title("Sales vs. Profit Density")
plt.show()
```
#### 3. Sales by Category & Region
```python
sns.catplot(x="Category", y="Sales", col="Region", data=df, kind="bar")
plt.show()
```

## 💡 Key Findings
- **Furniture has lower profitability** due to high discounts.
- **Technology products generate the highest profit margins**.
- **Standard Class shipping mode is the most used**, but Express options increase profitability.
- **Sales in the Western region are highest, while profit margins vary regionally**.

## 💼 Contributing
Contributions are welcome! Feel free to **fork** the repo, create a new branch, and submit a **pull request**.

## 🌟 Acknowledgments
- Dataset inspired by **Sample Superstore Data**.
- Libraries used: **Pandas, NumPy, Seaborn, Matplotlib**.

---
✨ **Let’s explore data and uncover business insights together!** 🚀

