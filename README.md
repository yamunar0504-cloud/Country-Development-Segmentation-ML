
🌍 Country Development Segmentation using Unsupervised Machine Learning

📌 Project Overview

This project applies unsupervised machine learning techniques to analyze and segment countries based on socio-economic and health indicators.

The dataset includes development factors such as income, GDP per capita, life expectancy, child mortality, exports, imports, healthcare expenditure, inflation rate, and fertility rate.

🎯 Goal:
Group countries with similar development characteristics using clustering algorithms.

Countries are segmented into development categories such as:

🟢 Developed Countries

🟡 Developing Countries

🔴 Underdeveloped Countries


This analysis helps policymakers and international organizations understand global development patterns and allocate resources effectively. 


---

🏢 Business Context

International development organizations and NGOs work with multiple countries that have different economic and social conditions.

Because resources and funding are limited, organizations must identify countries that require urgent assistance.

Machine learning can help automatically analyze development indicators and group countries with similar characteristics, enabling data-driven policy decisions and resource allocation. 


---

❗ Problem Statement

Countries across the world show large differences in economic strength, healthcare quality, and social development.

Some countries have strong economies, high life expectancy, and low child mortality, while others face economic instability and poor healthcare infrastructure.

The challenge is to analyze these indicators and cluster countries into meaningful groups based on development level. 


---

🎯 Project Objectives

✔ Analyze global development indicators
✔ Perform data preprocessing and exploratory data analysis
✔ Apply clustering algorithms to group similar countries
✔ Determine the optimal number of clusters using Elbow Method and Silhouette Score
✔ Profile clusters to understand development patterns
✔ Generate insights for global development planning 


---

📂 Dataset Description

The dataset contains socio-economic and health indicators for 167 countries.

Each row represents a country, and each column represents a development metric.

📊 Feature	Description

child_mort:	Child mortality rate

exports:	Exports as percentage of GDP

health:	Healthcare expenditure (% of GDP)

imports:	Imports as percentage of GDP

income:	Average income per person

inflation: Annual inflation rate

life_expec:	Life expectancy

total_fer:	Total fertility rate

gdpp: GDP per capita

country	Country name (identifier only)


The country column is not used for clustering, as it is only a categorical identifier. 

🔗 Dataset Link
https://drive.google.com/file/d/1nOV9cotScwoZz-Blb6c6Dk9A_XuKV-F_/view?usp=drivesdk

---

🧹 Data Preprocessing

Before applying clustering algorithms, the dataset was prepared by:

✔ Checking for missing values
✔ Removing duplicate records
✔ Standardizing features using StandardScaler

Feature scaling is essential for clustering because the algorithm relies on distance calculations between variables. 


---

📊 Exploratory Data Analysis (EDA)

EDA was performed to understand patterns in development indicators.

Key analyses included:

📈 Income distribution across countries
📊 Variation in child mortality rates
📉 Life expectancy distribution
🔗 Relationships between economic and health indicators

The analysis revealed:

Higher income is associated with higher life expectancy

Lower income countries tend to have higher child mortality rates 


---

🤖 Clustering Algorithms Used

🔹 K-Means Clustering

K-Means groups similar data points into clusters based on distance from cluster centroids.

Why K-Means was chosen:

✔ Works well with numerical datasets
✔ Efficient for large datasets
✔ Clearly separates country groups based on development indicators 


---

🔹 Hierarchical Clustering

Hierarchical clustering was also applied to analyze similarity between countries.

However, K-Means was selected as the final model due to better cluster separation and efficiency. 

---

📉 Determining Optimal Clusters

📊 Elbow Method

The Elbow Method evaluates clustering performance by plotting Within Cluster Sum of Squares (WSS) against different cluster values.

The optimal point occurred at:

🎯 K = 3


---

📏 Silhouette Score

Silhouette Score evaluates how well data points belong to their assigned clusters.

Scores ranged between 0.24 – 0.25, validating the choice of three clusters. 


---

🌍 Cluster Profiling

🟢 Cluster 1 — Developed Countries

Characteristics:

✔ Very high income
✔ High GDP per capita
✔ High life expectancy
✔ Low child mortality
✔ Strong healthcare systems

Examples: Canada, Australia, Austria


---

🟡 Cluster 0 — Developing Countries

Characteristics:

✔ Moderate income levels
✔ Improving healthcare systems
✔ Growing economies

Examples: Albania, Algeria, Armenia


---

🔴 Cluster 2 — Underdeveloped Countries

Characteristics:

✔ Low income levels
✔ High child mortality
✔ Low life expectancy
✔ Weak healthcare infrastructure

Examples: Afghanistan, Angola, Benin 


---

🔍 Key Insights

📌 Income and child mortality have a strong inverse relationship

📌 Wealthier countries have better healthcare systems and longer life expectancy

📌 GDP and healthcare spending are key indicators of development

📌 Underdeveloped countries face multiple economic and social challenges simultaneously 


---

💡 Recommendations

🌍 Support Underdeveloped Countries

International organizations should prioritize funding and development programs.

🏥 Improve Healthcare Infrastructure

Investing in healthcare can reduce mortality and increase life expectancy.

📈 Promote Economic Growth

Encourage foreign investment, trade opportunities, and industrial development.

🎓 Improve Education and Skills

Education and workforce development can accelerate economic progress.

📊 Use Data-Driven Policy Planning

Machine learning insights can guide resource allocation and development strategies. 


---

🛠 Tools and Technologies

💻 Programming Language

Python


📚 Libraries

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn


☁ Development Environment

Google Colab 



---

📁 Project Structure

Country-Segmentation-Unsupervised-ML

├── dataset
│   └── country_data.csv
│
├── notebook
│   └── country_segmentation_kmeans.ipynb
│
└── README.md


---

📌 Conclusion

This project demonstrates how unsupervised machine learning can segment countries based on economic, social, and health indicators.

Using K-Means clustering, countries were grouped into three development categories: developed, developing, and underdeveloped.

These insights can help governments and global organizations make data-driven decisions for development planning and resource allocation. 


