# Data-Driven Insights into Vehicle Pricing and Market Behavior

This project presents a comprehensive PESTEL-based analysis of the used car market using statistical modeling, regression analysis, and time-series forecasting techniques. The study analyzes more than 558,000 used vehicle transactions across the United States to understand how internal vehicle characteristics and external macro-environmental factors influence vehicle pricing trends.

## Academic Information
Course: DAMO-511-9 Data Analytics Case Study 2  
Program: Master of Data Analytics  
Institution: University of Niagara Falls, Canada  
Student: Sathiya Sampath  

## Project Objectives
- Analyze factors influencing used car prices
- Apply PESTEL framework to automotive market behaviour
- Build regression models to predict vehicle prices
- Perform ARIMA forecasting for future pricing trends
- Generate strategic insights for buyers, dealerships, and policymakers

## Dataset
Dataset: `car_prices.csv`

### Key Variables
- `sellingprice` → Final vehicle transaction price
- `year` → Vehicle manufacturing year
- `odometer` → Mileage driven
- `condition` → Vehicle condition rating
- `make`, `model`, `body`, `state` → Vehicle attributes
- `saledate` → Transaction date for time-series forecasting

## Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Statsmodels
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning & Preprocessing
The project includes:
- Standardization of text columns
- Missing value treatment
- Duplicate removal
- Outlier detection using IQR
- Date formatting and monthly aggregation
- Numeric conversion and unrealistic value filtering

## Exploratory Data Analysis (EDA)
EDA techniques used:
- Histograms
- Scatter plots
- Correlation heatmaps
- Boxplots
- Trend visualizations

### Key Insights
- Newer vehicles with lower mileage have higher resale values
- Vehicle condition positively affects selling price
- Mileage negatively impacts vehicle pricing
- Market prices remain relatively stable over time

## Regression Analysis
A Multiple Linear Regression model was developed:

SellingPrice = β0 + β1(Year) + β2(Odometer) + β3(Condition) + ε

### Results
- Adjusted R² = 0.391
- Vehicle year positively influences price
- Higher mileage reduces resale value
- Better vehicle condition increases selling price

### Model Diagnostics
- Residual analysis
- Variance Inflation Factor (VIF)
- Durbin-Watson Test
- Residual vs Fitted plots

## Time-Series Forecasting
ARIMA models were used to forecast future average used-car prices.

### Forecast Findings
- Average used-car prices are expected to remain stable
- Forecasted monthly values range between $16,161 and $16,294
- No significant short-term price volatility observed

## PESTEL Analysis

### Political Factors
- Government policies and EV incentives affect resale values

### Economic Factors
- Inflation, fuel prices, and interest rates influence demand

### Social Factors
- Consumer preferences impact vehicle type demand

### Technological Factors
- Advancements in EVs and smart vehicle technology affect depreciation

### Environmental Factors
- Emission regulations impact older vehicle resale prices

### Legal Factors
- Consumer protection laws influence market transparency

## Business & Strategic Implications

### For Consumers
- Focus on low-mileage, well-maintained vehicles for better value

### For Dealerships
- Prioritize fuel-efficient and newer inventory

### For Policymakers
- Balance environmental regulations with affordability concerns

### For Manufacturers
- Build vehicles with long-term resale value and sustainability focus

## Limitations
- Missing variables such as accident history and fuel type
- Short-term forecasting horizon
- Regression limited to linear relationships
- Regional market differences not included

## Future Improvements
- Add categorical encoding for make, body, and fuel type
- Apply machine learning models
- Explore regional segmentation analysis
- Build advanced predictive forecasting models
  
## Conclusion
This project demonstrates how data analytics, statistical modeling, and PESTEL analysis can be combined to generate actionable insights into used vehicle pricing trends,
market stability, and strategic decision-making in the automotive resale industry.

## Repository Structure

```text
used-car-market-pestel-analysis/
│
├── data/
├── notebooks/
├── visualizations/
├── reports/
├── README.md
├── requirements.txt
