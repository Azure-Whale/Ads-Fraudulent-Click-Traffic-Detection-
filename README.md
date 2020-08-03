# Ads-Fraudulent-Click-Traffic-Detection
## Goal
Our study aims to learn if there is any potential undiscovered symptoms that people would like to share on their social media. The data is gained from Tweet API which enables us to gain daily tweet. We saved those on the server. By extracting and visualizing these data, we try to learn things behind these daily tweets.
## Data Collection
The data is collected using Tweet API, and we only colletec tweets data about COVID-19
## EDA
To find the correlation between time and click-count & click through
1. Sampling data
2. Handle Missing Value
## Feature engineering
Extrac time related features according to EDA, say weekly click-count, interval between clicks from same user and etc.
### Click-count vs Time Series 1
![R0](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R0.png)
### Click-count vs Time Series 2
![R1](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R1.png)
### Click-count Distribution
![R2](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R2.png)
## Methos
• Performed EDA (Exploratory Data Analysis) on 10GB+ clicks data from mobile devices and preprocess the raw data via dealing with
missing values, categorical feature encoding; identify unique user click by tracking clicks from same IP address, OS and ad channel
• Conducted feature extraction by transforming raw time data into multiple high-quality features such as click interval, weekly clicks
• Built LightGBM model via k-fold cross validation, evaluated prediction results with ROC AUC (0.97) and identified key factors 
## Results
![R](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/Results.png)

