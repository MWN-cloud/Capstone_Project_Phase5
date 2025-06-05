**Modeling Economic Growth: Singapore’s Insights for Kenya**

**Overview**

This project applies time series and machine learning models to Singapore's economic indicators with the aim of drawing insights and building models that Kenya can adapt for GDP forecasting and policy planning.

**Business Problem**

Kenya seeks to improve its economic forecasting and policy design. This project leverages the successful economic structure of Singapore to develop forecasting models that predict Kenya's GDP based on key production-related indicators. The goal is to provide reliable GDP predictions that can inform government planning, budgeting, and investment prioritization.

**Business Objectives**

1.Compare sectoral contributions to GDP in Singapore and Kenya to identify similarities in growth-driving industries.

2.Model the Relationship Between Economic Inputs and Output

3.Identify High-Impact Policies Behind Singapore’s Economic Transformation

4.Develop and deploy an interactive dashboard to forecast sub-sector growth andestimate their contributions to overall GDP.

**Datasets and Features**

   **Data Sources:** 

1. Singapore Department of Statistics
2. Central Bank of Kenya – Statistics
3. World Bank
   
   **Datasets:**

•	Singapore's GDP Production & GDP vs  Debt Data (1960 -2024) - D
•	Kenya’s production Data (2018-2022) – for sector comparison, 
•	Kenya’s Debt vs GDP Data – from World Bank

   **Target Variable:** `GDP (current market prices)

   **Key Predictors:**  manufacturing, Finance and Insurance, wholesale & retail traded, transportation & storage and education. 



**Tools and Libraries**

•	- Python
•	- pandas, numpy
•	- matplotlib, seaborn
•	- scikit-learn
•	- statsmodels (SARIMAX, VAR)
•	- Jupyter Notebook


**Data Cleaning and Understanding**

•	Null values were filled with mean for normally distributed sectors and with median for non-normally distributed sectors
•	Outliers and duplicate entries were identified and resolved

**Exploratory Data Analysis**

We were able to Identify top performic Sectors in Singapore i.e. wholesale trade, manufacturing, finance and insurance and transportation and storage.
![image](https://github.com/user-attachments/assets/30145171-b65e-4c11-99f2-dfa260fb67be)

 
We also identified top performing sectors in Kenya for comparative reasons  i.e. agriculture, transportation and storage, real estate, taxes on products, wholesale and retail trade and finance and insurance activities. 
![image](https://github.com/user-attachments/assets/01451d73-002e-40df-b020-7124b7186b2b)

 
We focused on sectors common to both countries for modeling i.e. transporation and storage, wholesale and retail trade financial services and manufacturing

We also visualized the sectors with the highest year-on-year growth to identify the strategies and policies driving this exponential increase.
![image](https://github.com/user-attachments/assets/c1dfe8a3-1e89-44ed-8841-0bd16a7df703)

 
We also visualized GDP growth over time for both countries
![image](https://github.com/user-attachments/assets/a957838d-b06e-4bd3-8ce7-373707a26a3e)

 


**Pre-processing and Modeling**

Our approach combined regression and time series models to predict GDP, along with clustering techniques to anticipate policy reforms within specific groups

**1. Time Series Models**

•	SARIMAX: Incorporates time trend exogenous predictors
•	VAR: Models interactions among multiple time series variables

**2. Regression Models**

•	Multiple Linear Regression
•	Support Vector Regression (SVR)
•	Decision Tree Regressor
•	Random Forest Regressor
•	GradientBoostingRegressor
•	KNeighborsRegressor

**3.  Deep Learning Model**

•	GRU (Gated Recurrent Unit)

**4. Clustering**

•	K Means Clustering


**Model Evaluation**

The below was the performance of the models; With the key focus variables being r-squared and RMSE for regression models and MAPE and MAE for Time Series models
 

•	RNN model had the best performance with 1% variance between predicted and actual and a mean absolute error of 4564.59 which is a very lower error compared to the magnitude of the values of GDP 
•	KNN emerged as the best-performing regression model, achieving up to 99.6% prediction accuracy and a low RMSE of 0.1194, indicating minimal errors.
•	The Multiple Linear Regression was used to identify the correlation of specified sector as above in order to predict gdp growth if specified policies are applied
•	Clustering revealed year-based patterns tied to identify key strategies and policies, helping trace Singapore’s path to its current status

**Policies relating to the Key Sectors;**

**Finance and Insurance**

Cluster 1 (1960–1987):
•	Introduced offshore banking (1968) and allowed foreign currencies.
•	Opened to insurance firms; aligned legal frameworks with global standards.
•	Launched the Singapore Stock Exchange.
Cluster 2 (1988–2009):
•	Attracted global banks for private banking.
•	Gradually removed restrictions on foreign bank branches.
Cluster 3 (2010–2024):
•	Enabled regulated crypto-asset services.
•	Formed bilateral capital flow agreements (e.g., China, India, UK).

**Manufacturing**

Cluster 1 (1960–1987):
•	Established first industrial zone (1961) to attract MNCs.
•	Set up vocational training (e.g., Industrial Training Board, 1968).
•	Partnered with foreign firms for industry-aligned skills.
Cluster 2 (1988–2009):
•	Focused on high-tech sectors: semiconductors, biomedical, aerospace.
•	Attracted scientists, start-ups, and R&D labs.
Cluster 3 (2010–2024):
•	Targeted Industry 4.0 (smart manufacturing, 3D printing).
•	Invested in biotech, semiconductors, aerospace.
•	Rolled out SkillsFuture (2015) for workforce re-skilling.

**Transportation and Storage**

Cluster 1 (1960–1987):
•	Centralized and modernized port operations.
•	Integrated road, port, and warehouse systems.
Cluster 2 (1988–2009):
•	Built logistics parks and bonded warehouses.
•	Began planning for MRT-road-freight integration.
Cluster 3 (2010–2024):
•	Launched automated container ports (first in 2021; full by 2040).
•	Promoted cargo tracking and blockchain in trade logistics.

**Wholesale and Retail Trade**

Cluster 1 (1960–1987):
•	Established free trade zones; supported re-export/logistics.
•	Reduced tariffs and trade barriers.
Cluster 2 (1988–2009):
•	Singapore supported SME exports.
•	Liberalized market entry for foreign brands.
Cluster 3 (2010–2024):
•	Promoted smart retail (AI, AR, RFID).
•	Provided grants for SME digitalization (e.g., Shopify, Lazada)

**Future Work**

•	Adapt model for real Kenyan economic data.
•	Include additional macroeconomic indicators (inflation, interest rates).
•	Develop a real-time dashboard for policymakers.

**Limitations**

1.	Lack of congruent data
2.	The policy implication is subject to multiple conditions that may not directly translate tothe figures modeled

 **Authors**

•	Kirui Wilberforce 
•	Charity Nguru
•	Maureen Ngahu
•	Neema Elaly
•	Kiprono Bett
•	Jael Kirwa
