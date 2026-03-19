📊 Airbnb Price Prediction Project


🔍 Project Overview

This project focuses on predicting Airbnb listing prices in New York City using real-world data.
The goal is to estimate listing prices based on features such as location, availability, reviews, and host-related attributes.

🧹 Data Preprocessing

Removed unnecessary and non-informative features (e.g. names, IDs).

Handled missing values using simple imputation (filled with 0 where appropriate).

Applied:


One-Hot Encoding for categorical features


Standard Scaling for numerical features


Also handled outliers by capping extreme price values and applied log transformation to stabilize the target variable.


🛠️ Feature Engineering

A large part of the project focused on creating meaningful features, including:


Demand-related features (reviews, availability ratios)


Location-based features (distance from city center)


Host activity features


Binning latitude and longitude


Combining categorical features (e.g. room type + location)


At some point, results became inconsistent and hard to interpret, which led me to experiment with KMeans clustering to group locations and extract additional spatial patterns.


🤖 Modeling Approach

Multiple models were tested and tuned using GridSearchCV.

The main focus was on improving generalization and reducing overfitting rather than just increasing training performance.


📈 Results Summary

The best performance achieved:


R² Score ≈ 0.63


RMSE and MAE showed stable but limited improvements


Despite multiple attempts (feature engineering, tuning, model adjustments), improvements became marginal after a certain point.


🧠 Key Challenges


High noise in the dataset


Missing important real-world factors (images, quality, descriptions)


Overfitting in more complex models


Small improvements despite heavy tuning


Feature engineering had a bigger impact than model choice


🚀 Conclusion

This project represents a full end-to-end regression pipeline, including preprocessing, feature engineering, model tuning, and evaluation.


The results are decent, but honestly, I’m not fully convinced they represent the best possible outcome.

However, I put significant effort into experimenting, analyzing, and pushing the model as far as I could with the available data.


This project was a strong learning experience in dealing with real-world data limitations and model behavior.



Author

Ameen Nasairah
