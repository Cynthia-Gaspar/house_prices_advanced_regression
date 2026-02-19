#  🏠 Ames Housing: Advanced Regression Techniques

## 📌 Executive Summary

Accurate property valuation is essential for real estate investment, mortgage lending, property tax assessment, and insurance underwriting. This model demonstrates how data science can transform raw housing data into reliable price estimates, enabling better decision-making across the real estate ecosystem.

This project aims to develop a **machine learning model to predict residential property prices** using data from Ames, Iowa. By analyzing 79 different housing characteristics, the model learns patterns that drive property values and applies them to predict prices on unseen data.

---

## 📊 Data Information

The dataset comes from the **Ames Housing dataset**, a modern alternative to the classic Boston Housing data, compiled by Dean De Cock for data science education.

| Characteristic | Description |
|----------------|-------------|
| **Time Period** | Properties sold in Ames, Iowa between 2006–2010 |
| **Training Set** | 1,460 properties with known sale prices |
| **Test Set** | 1,459 properties for final prediction |
| **Features** | 79 explanatory variables describing lot characteristics, structural components, interior features, and neighborhood attributes |

---

## 📈 Key Results

### Performance Summary

| Model | Validation Error (log-RMSE) | Business Interpretation |
|-------|------------------------------|------------------------|
| **Weighted Ensemble** | **0.1275** | 🏆 **Best performer — 12.8% average error** |
| Ridge Regression | 0.1314 | Very strong — 13.1% average error |
| Lasso Regression | 0.1321 | Strong — 13.2% average error |
| ElasticNet | 0.1324 | Strong — 13.2% average error |
| Gradient Boosting | 0.1375 | Good — 13.8% average error |

### What This Means for Business

A **12.8% average prediction error** means that for a **$300,000 home**, the model's prediction would typically be within approximately **$38,400** of the actual sale price. This level of accuracy is competitive with human appraisals, while being **faster, more consistent, and easily scalable**.

### The Ensemble Advantage

The weighted ensemble **improved accuracy by 3.0%** over the best individual model (Ridge). In business terms:

| Metric | Improvement |
|--------|-------------|
| **Error reduction** | From 13.1% → 12.8% |
| **Dollar impact** | $390 better prediction on a $300,000 home |
| **Risk reduction** | More stable, reliable valuations across all price ranges |

---

## 🛠️ Technologies Used

| Category | Technologies |
|----------|--------------|
| **Programming** | Python 3.8+ |
| **Data Processing** | Pandas, NumPy, Patsy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-learn (Lasso, Ridge, ElasticNet), Statsmodels, XGBoost (fallback to HistGradientBoosting) |
| **Development** | Jupyter Notebook, VS Code |
| **Version Control** | Git, GitHub |

---

## 🧭 Reflection and Learnings

This project gave me hands-on experience with the full machine learning pipeline — from raw data to a deployable model. Some of my key takeaways:

- **Feature Engineering:** learned how domain knowledge (in this case, understanding what makes a house valuable) directly impacts model performance.
- **Regularized Regression:** developed intuition for when to use Lasso vs. Ridge vs. ElasticNet and how each handles multicollinearity differently.
- **Ensemble Methods:** discovered that combining models thoughtfully outperforms any single model, even well-tuned ones.
- **Communicating results:** practiced translating technical metrics into business language — a skill I find just as important as the modeling itself.

This work was developed as part of my Management Analytics Master's program at Queen's University.

---

## 👩‍💻 About the Author

Hi! I'm Cynthia Gaspar, a business professional pursuing a Master's degree in Management Analytics at Queen's University. I am passionate about understanding real-world problems through data. Let's connect!

🔗 [LinkedIn](https://www.linkedin.com/in/cynthia-gaspar)
🔗 [Substack](https://substack.com/@cynthiagaspar)
