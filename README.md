# lsd-cognitive-performance-regression

# 📊 Correlation of LSD Tissue Concentration and Cognitive Performance  
### A Linear Regression Analysis Based on Wagner et al. (1968)

This project explores the relationship between **tissue concentration of LSD-25** and **average arithmetic test performance** in human subjects.  
Using linear regression, we evaluate how increasing LSD concentration affects cognitive function.

This notebook is designed to demonstrate:

- Exploratory data analysis (EDA)  
- Data visualization  
- Linear regression modeling  
- Interpretation of statistical results  
- Reproducible scientific workflow  

---

## 📁 Project Structure

├── LSD_Analysis.ipynb # Jupyter Notebook (main analysis)
├── lsd_math_score_data.csv # Dataset (Wagner et al., 1968)
└── README.md # Project documentation

---

## 📘 Background

The dataset comes from the study:  
**"Correlation of performance test scores with tissue concentration of lysergic acid diethylamide in human subjects" (Wagner et al., 1968)**

The experiment measured:

- **Tissue concentration of LSD (ppm)**
- **Time after administration (minutes)**
- **Average math test performance**

**Hypothesis:** Increasing LSD concentration leads to decreased cognitive performance.  
This project validates that hypothesis using regression analysis.

---

## 🧪 Methods

### 1. **Exploratory Data Analysis**
- Line plot of tissue LSD concentration over time  
- Data inspection (`head()`, `describe()`)  

### 2. **Regression Modeling**
We fit a simple linear regression model:

\[
\text{Score} = \theta_0 + \theta_1 \cdot \text{(LSD concentration)}
\]

### 3. **Performance Metrics**
- Regression coefficient (θ₁)  
- Intercept  
- R² score  

### 4. **Visualization**
- Scatter plot of test score vs LSD level  
- Regression line visualization  

---

## 📈 Key Results

| Metric | Value |
|-------|--------|
| **Slope (θ₁)** | -9.009 |
| **Intercept** | 89.124 |
| **R² Score** | 0.878 |

### Interpretation:
- For every **+1 ppm increase in LSD**, math performance **drops by ~9 points**.  
- R² = 0.878 means the model explains **87.8% of score variation**.  
- Strong negative correlation → higher LSD concentration significantly reduces cognitive ability.

---

## 📊 Visualizations

### LSD Concentration Over Time
Shows how LSD tissue levels change after administration.

### Regression Model
Scatter of actual performance vs. LSD concentration  
Regression line showing predicted scores.

(See notebook for figures.)

---

## 🚀 How to Run This Project

### 1. Clone the repository

git clone https://github.com/bmirzo/lsd-cognitive-performance-regression.git
cd lsd-cognitive-performance-regression

### 2. Install dependencies
pip install -r requirements.txt

(Or manually install: pandas, matplotlib, scikit-learn)

### 3. Open the notebook
jupyter notebook LSD_Analysis.ipynb

🛠️ Technologies Used

Python 3

pandas

matplotlib

scikit-learn

Jupyter Notebook

📚 References

Wagner, J. G., Amsel, L. P., & Schanker, L. S. (1968).
Correlation of performance test scores with tissue concentration of lysergic acid diethylamide in human subjects.
