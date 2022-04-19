# Clustering_Apriori
Customer Personality Analysis: Predict customer who will most likely buy wine (Personal Project)
•	Data: Open Source
•	EDA: graphed variables (30c, 3000rows), looked at birth year, education level, etc. using bar charts and histograms
•	Created features to define customer personalities: Spending habits, seniority level, 
•	Removed outliers (based on graphs, could use Shapiro-wilks)
•	Normalize Data: Using the standardscaler, normalized income, seniority, spending 
•	Clustering: Using Gaussaian mixture, created clusters defined segments as: 
    Stars- prev. customer, high income, high spending
    Need att- new, low income, low spending
    High potential-new, high income, high spending
    Leaky bucket- old, low income, lowspedning
•	Data Prep for Apriori: 
    defined three segments based on age, income, seniority
    defined new segments according to the spending of customers on each product (nonbuyer, lowbuyer, frequent buyer, biggest buyer)
•	Aprior: Used this because it’s the simplest technique to identifying underlying relationships: all nonempty substes of a freq. cat. Must also be freq. – we want to identify biggest customer of wines. Used get_dummies on association, aprirori(), association_rules()
•	Conclusion: Customers with average income around 70,000 who spend 1300, previous customer for 20 months, education level of a graduate degree, and buy meats
