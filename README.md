# Customer Purchase Behavior Analysis using Descriptive Statistics

## 📊 Project Overview
Welcome to the **Customer Purchase Behavior Analysis** project! This project applies probability and statistical concepts to a real-world dataset to uncover patterns and relationships in customer purchasing behavior. The goal is to identify actionable insights that can optimize marketing strategies and boost offer acceptance rates.

---

## 🔍 Problem Statement
Our company aims to enhance its marketing efforts by better understanding customer purchase patterns. This project focuses on analyzing customer data to:
- Identify key demographics and spending behaviors.
- Explore relationships between customer attributes and purchasing habits.
- Segment customers into meaningful groups for targeted marketing.

The dataset includes information about customer demographics, spending history, and engagement across multiple purchase channels (store, web, catalog).

---

## 🎯 Objectives
1. **Data Cleaning and Preprocessing:**
   - Handle missing values and ensure data type consistency.
   - Detect and treat outliers without losing valuable insights.
2. **Descriptive Statistics:**
   - Calculate central tendency measures (mean, median, mode).
   - Analyze data spread through variance and standard deviation.
3. **Probability Distributions:**
   - Identify variables aligning with probability distributions (e.g., Binomial, Poisson).
   - Calculate probabilities and expected values for key metrics.
4. **Customer Segmentation:**
   - Segment customers based on income, spending, and engagement levels.
   - Label high-value customers for personalized marketing.
5. **Business Recommendations:**
   - Provide data-driven strategies for targeted marketing, customer retention, and pricing optimization.

---

## 📦 Dataset Description
The dataset contains the following key variables:

- **Response (target):** 1 if customer accepted the offer, 0 otherwise.
- **ID:** Unique customer ID.
- **Year_Birth:** Customer's year of birth.
- **Complain:** 1 if the customer complained in the last 2 years.
- **Dt_Customer:** Date of customer enrollment.
- **Education:** Level of education.
- **Marital:** Marital status.
- **Kidhome:** Number of small children.
- **Teenhome:** Number of teenagers.
- **Income:** Yearly household income.
- **MntFishProducts:** Amount spent on fish in the last 2 years.
- **MntMeatProducts:** Amount spent on meat in the last 2 years.
- **MntFruits:** Amount spent on fruits in the last 2 years.
- **MntSweetProducts:** Amount spent on sweets in the last 2 years.
- **MntWines:** Amount spent on wine in the last 2 years.
- **MntGoldProds:** Amount spent on gold products.
- **NumDealsPurchases:** Number of discount purchases.
- **NumCatalogPurchases:** Number of catalog purchases.
- **NumStorePurchases:** Number of store purchases.
- **NumWebPurchases:** Number of web purchases.
- **NumWebVisitsMonth:** Number of website visits in the last month.
- **Recency:** Days since last purchase.

---

## 📊 Tasks & Methodology
### 1️⃣ Data Cleaning & Preprocessing
- **Handling Missing Values:**
  - Imputed missing income using a calculated approach: `Total Purchase Amount / Mean Purchase Income Ratio`.
  - Placeholder dates in `Dt_Customer` were replaced with `NaT`.
- **Data Type Consistency:**
  - Converted `Year_Birth` to datetime.
  - Calculated **Age** from `Year_Birth`.
- **Outlier Detection:**
  - Used Z-score method (threshold: 3 standard deviations).
  - Removed implausible ages (above 100).
  - Retained high-value customers ("High Spenders" and "Frequent Buyers").

### 2️⃣ Descriptive Statistics
- **Central Tendency:**
  - Mean, Median, and Mode for Age, Income, Spending amounts.
- **Dispersion Metrics:**
  - Variance and Standard Deviation.
- **Data Visualization:**
  - Histograms, Boxplots, and Pie Charts to highlight spending patterns and demographics.

### 3️⃣ Probability Distributions
- Assessed key variables for distribution alignment:
  - **NumWebVisitsMonth:** Poisson distribution.
  - **NumDealsPurchases, NumCatalogPurchases, NumStorePurchases:** Binomial distribution.
- **Probability Calculations:**
  - Computed probabilities of key purchasing behaviors.

### 4️⃣ Customer Segmentation
- **Income and Spending Segments:**
  - Low-Income, Low Spenders
  - Middle-Income (Low & High Spenders)
  - High-Income (High Spenders & Untapped Potential)
- **Behavioral Labels:**
  - "High Spenders" (top 5% of spenders).
  - "Frequent Buyers" (top 5% of purchase frequency).

### 5️⃣ Insights & Recommendations
- **Income and Spending:**
  - Positive correlation between income and spending.
  - Web visits show negative correlation with total spending.
- **Targeted Marketing:**
  - **Low-Income Segment:** Loyalty programs and discounts.
  - **High-Income Segment:** Premium offers and personalized experiences.
- **Customer Retention:**
  - Implement tiered loyalty programs.
- **Website Optimization:**
  - Enhance mobile experience.
  - Introduce AI-powered product recommendations.
- **Pricing Strategy:**
  - Explore dynamic pricing models.
  - Conduct price sensitivity analysis.

---

## 📈 Results
- **High Spenders and Frequent Buyers:** Identified and tagged, helping design personalized marketing campaigns.
- **Segmentation:** Successfully grouped customers by income and spending patterns.
- **Data-Driven Insights:** Provided actionable insights for targeted offers, loyalty programs, and optimized marketing strategies.

---

## 🚀 Conclusion
By leveraging descriptive statistics, probability distributions, and customer segmentation, this project reveals critical insights into customer behavior. These insights empower businesses to:
- Improve marketing efficiency.
- Personalize customer experiences.
- Boost offer acceptance rates.

The next steps include integrating predictive modeling for dynamic segmentation and enhancing customer relationship management (CRM) strategies.

---

## 🛠️ Tools & Technologies
- **Python**: Pandas, NumPy, Matplotlib, Seaborn
- **Statistics**: Descriptive statistics, Probability distributions
- **Visualization**: Histogram, Boxplot, Pie Chart
- **Modeling**: Binomial and Poisson distribution analyses

---

## 📚 How to Use
1. **Clone this repository:**
```bash
git clone https://github.com/yourusername/Customer-Purchase-Behavior-Analysis.git
```
2. **Install dependencies:**
```bash
pip install -r requirements.txt
```
3. **Run the analysis:**
```bash
python analysis.py
```
4. **Explore the visualizations and reports** in the `outputs/` folder.

---

## ✨ Acknowledgments
Special thanks to the mentors for their guidance and support. This project was inspired by real-world marketing challenges and aims to bridge the gap between data science and business strategy.

---

Feel free to reach out for collaborations or feedback! 🚀
