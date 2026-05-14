# AeroFit Treadmill Customer Profiling & Exploratory Data Analysis (EDA)

## 📌 Project Overview

The market research team at AeroFit aims to identify the specific characteristics of the target audience for each of their three treadmill models: KP281, KP481, and KP781. The goal of this project is to investigate differences across customer demographics and provide data-driven recommendations to help AeroFit better target new customers and optimize their product recommendations.

## 🗄️ Product Portfolio & Dataset

The dataset (`aerofit_treadmill_data.csv`) contains three months of prior sales data regarding individuals who purchased an AeroFit treadmill.

**Treadmill Models:**

* **KP281:** Entry-level treadmill, priced at $1,500.
* **KP481:** Mid-level runner treadmill, priced at $1,750.
* **KP781:** Advanced feature treadmill, priced at $2,500.

**Customer Variables (Features):**

* `Product`: Model purchased (KP281, KP481, or KP781)
* `Age`: Customer age in years
* `Gender`: Male / Female
* `Education`: Years of education
* `MaritalStatus`: Single or Partnered
* `Usage`: Average expected weekly usage
* `Fitness`: Self-rated fitness score (1 = Poor, 5 = Excellent)
* `Income`: Annual income in USD
* `Miles`: Expected average miles to walk/run per week

## 🛠️ Tools & Libraries Used

* **Python:** Core language for the analysis
* **Pandas & NumPy:** Data manipulation, aggregation, and statistical summaries
* **Matplotlib & Seaborn:** Data visualization (Distribution, Count, Box, Pairplots, Heatmaps)

## 📊 Analysis Methodology

This project follows a structured exploratory data analysis pipeline:

1. **Data Exploration & Processing:** Initial data ingestion, checking shapes, data types, missing values, and handling duplicate entries.
2. **Statistical Summary:** High-level descriptive statistics for both categorical and numerical variables.
3. **Non-Graphical Analysis:** Value counts and unique attribute mapping for categorical features.
4. **Graphical Analysis:** * *Univariate:* Distributions, count plots, and box plots to understand individual variables.
* *Bivariate:* Assessing how features (Gender, MaritalStatus, Age, etc.) impact the specific Product purchased.
* *Multivariate:* Pairplots mapping relationships across multiple dimensions.


5. **Correlation Analysis:** Heatmaps to uncover linear relationships between numerical features (e.g., Fitness vs. Miles).
6. **Outlier Detection:** Identifying anomalies in Income or Miles using the Interquartile Range (IQR) method.
7. **Probability Profiling:** Calculating marginal and conditional probabilities to answer specific business questions.

## 💡 Key Business Insights

* **Product Popularity & Demographics:** The KP281 is the most popular product overall. The majority of the customer base is partnered, between the ages of 25 and 30, and has completed high school or some college education.
* **Income Tiers:** The KP281 and KP481 models are highly popular with customers in the $45,000–$60,000 income range.
* **Premium Model Preferences:** Customers with higher education levels and frequent usage expectations tend to prefer the advanced KP781 product.
* **Usage & Fitness:** Most customers plan to use the treadmill 3–4 times per week and perceive their fitness level as high (between 4–5).
* **Correlations:** There is a strong positive correlation between miles run and fitness level, alongside a moderate positive correlation between income and miles run. Ultimately, customers with higher incomes tend to run more miles.

## 🚀 Strategic Recommendations

1. **Capitalize on the Young Adult Market:** Since the KP281 and KP481 models are popular within the $45,000–$60,000 income range, they should be heavily marketed as affordable, high-value models. AeroFit should specifically target marketing campaigns toward young adults in their late 20s and early 30s to capitalize on this core demographic.
2. **Targeted Premium Positioning:** The KP781 should be explicitly marketed as a Premium Model. Advertising for this treadmill should be highly targeted toward specific segments of the customer base, namely high-income individuals, fitness enthusiasts, and those with advanced education levels who are more likely to run higher weekly mileage.
3. **Family-Centric Product Development:** Because a major segment of the customer base is partnered (indicating they are more likely to have or build families), future product development efforts should focus on features that cater to multi-user family groups, such as multiple user profiles or family-friendly safety features.

## 💻 How to Run This Project

1. Clone this repository:
```bash
git clone https://github.com/Hammy2112/AeroFit-Treadmill-EDA.git

```


2. Ensure you have Python installed along with Jupyter Notebook.
3. Install the required dependencies:
```bash
pip install pandas numpy matplotlib seaborn

```


4. Open the Jupyter Notebook (`EDA__Portfolio__Assignment_+_Report__Hassaan_Ahmed.ipynb`) to view the full code, visualizations, and thought process.
