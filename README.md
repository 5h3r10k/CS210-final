# CS210-final

## **Movies Data Analysis and Prediction**

This project is a comprehensive analysis of a movies dataset, with visualizations and a predictive model to forecast movie revenue based on specific features. It leverages Python libraries like pandas, matplotlib, and scikit-learn to clean data, visualize trends, and build predictive models.

---

### **Project Features**
1. **Data Cleaning**:
   - Removed missing or invalid entries for critical features such as `runtime`, `budget`, and `revenue`.
   - Filtered out invalid release years.

2. **Exploratory Data Analysis**:
   - **Key visualizations**:
     - **Average runtime of movies by release year**.
     - **Distribution of revenue across years**.
     - **Budget trends over time**.
   - Used matplotlib to present trends and insights.

3. **Predictive Model**:
   - A **Linear Regression model** built using `scikit-learn` predicts movie revenue.
   - Features used for prediction:
     - `release_year`
     - `runtime`
     - `budget`
     - `vote_average`
   - Model evaluation using the R² score.

4. **Prediction Example**:
   - Predicted revenue for a hypothetical movie with:
     - Release year: 2022
     - Runtime: 120 minutes
     - Budget: $10,000,000
     - Vote average: 7.5

---

### **Installation**

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   ```
2. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   ```
   Key dependencies include:
   - `pandas`
   - `matplotlib`
   - `scikit-learn`

3. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook CS210_final.ipynb
   ```

---

### **Usage**

1. **Run the notebook** to execute all cells sequentially for data analysis and visualization.
2. **Modify predictive features** in the model section to predict revenue for custom movie scenarios.

---

### **Example Prediction**

```python
# Example features
release_year = 2022
runtime = 120
budget = 10_000_000
vote_average = 7.5

# Predicted revenue
predicted_revenue = model.predict([[release_year, runtime, budget, vote_average]])
print(f"Predicted revenue: {predicted_revenue}")
```

---

### **Output Highlights**

- **R² Score**: The model achieved a score of `0.5509`, indicating moderate predictive power.
- **Predicted Revenue for Example**: $26,244,374.

Feel free to run and modify the notebook for further insights or enhancements to the predictive model.