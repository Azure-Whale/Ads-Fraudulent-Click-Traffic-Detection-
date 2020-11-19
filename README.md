# Ads-Fraudulent-Click-Traffic-Detection
## Goal
Prevent click fraud for app developers by measuring and detecting  user’s click across their portfolio, and flag IP addresses who produce lots of clicks, but never end up installing apps. Fraudulent click traffic may bring unnecessary cost on advertisement investment.
## Data
The data source is provided bt Talking Data. China’s largest independent big data service platform, covers over 70% of active mobile devices nationwide. They handle 3 billion clicks per day, of which 90% are potentially fraudulent. The data could be downloaded from https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection
## Steps
•	Performed EDA (Exploratory Data Analysis) on 40GB+ clicks data from mobile devices and preprocess on outliers and missing value 

•	Built meta-classifier (LR, LightGBM, CNN) to identify fraudulent click and explore important factors that affect ads conversion rate based on context features (IP, app channels, device...) & user behavior features (click frequency under different group-by conditions)

•	Conducted feature extraction by transforming raw time data into multiple high-quality features such as click interval, weekly clicks

•	Built meta-classifier via hyper-parameters tuning and 5-fold cross validation, finally get ROC AUC (0.97) and identified key factors 
## Feature engineering
Extrac time related features according to EDA, say weekly click-count, interval between clicks from same user and etc.
### Click-count vs Time Series 1
![R0](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R0.png)
### Click-count vs Time Series 2
![R1](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R1.png)
### Click-count Distribution
![R2](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/R2.png)
## Results of model
![R](https://github.com/Azure-Whale/Ads-Fraudulent-Click-Traffic-Detection-/blob/master/Results.png)
## Conclusion
It turns out that after the fine-tunning on the parameters as well as the correct feature extractions, the embedded models reach a high accuracy which is 97%. The model I trained has a strong confidence to predict users who are cheating on ads clicks

