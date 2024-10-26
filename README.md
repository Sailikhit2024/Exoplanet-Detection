Project Report: Exoplanet Hunting Using Machine Learning
Overview:
This project applies machine learning to identify potential exoplanets from flux
measurements of stars, utilizing the Kepler Space Telescope data. The main goal is to
distinguish between stars that host exoplanets and those that do not based on their light
intensity patterns.
Data Source:
The dataset includes flux intensity readings from 3,198 stars, classified into two groups:
potential exoplanet hosts and non-hosts, made publicly available by NASA.
Methodology:
1. Data Preprocessing:
- Conversion of LABELS to binary values: 1 (represents exoplanet) and 0 (does not
represent exoplanet).
- Memory usage of the data frame was reduced from 13.91 MB to 6.25 MB, a decrease of
55.1%, enhancing computational efficiency.
- Data normalization and Gaussian filters were applied to prepare the dataset for machine
learning models.
2. Feature Engineering:
- Implemented PCA for dimensionality reduction, decreasing feature dimensions to 37
principal components that retained around 98.8% of the original data variance.
- Addressed class imbalance using SMOTE, equalizing the distribution between the two
classes.
3. Model Development:
- Trained Support Vector Machines (SVM) and Random Forest models, with the SVM
achieving a mean cross-validation accuracy of approximately 91.86%.
- An Artificial Neural Network (ANN) built using Keras, also demonstrated a mean accuracy
of about 91.86% on the resampled dataset through 5-fold cross-validation.
Evaluation:
- Evaluated models based on precision, recall, F1-score, and accuracy, with significant
metrics indicating high effectiveness in predictions.
- Feature importance analysis for the Random Forest model identified critical features
contributing to exoplanet detection.
