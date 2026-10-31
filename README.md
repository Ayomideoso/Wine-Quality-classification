Wine Quality Classification

Project Overview

I created this project to sort red wines into good- and bad-quality groups based on their physicochemical features.

Wines scoring 7 or 8 are considered good, while those with scores from 3 to 6 are considered bad.

One challenge was that good-quality wines made up a much smaller part of the dataset. To address this, I used balanced accuracy, recall, and F1-score, in addition to overall accuracy, to evaluate the models.

Technologies

Python | Pandas | NumPy | Matplotlib | Scikit-learn | Random Forest | Support Vector Machine | GridSearchCV

Approach

* Inspected the dataset for missing values, duplicates and class distribution.
* Removed 240 exact duplicate records.
* Created a binary good/bad wine-quality target.
* Used a stratified train/test split to preserve class proportions.
* Built a Dummy Classifier as a baseline.
* Trained a class-balanced Random Forest model.
* Built an SVM pipeline with StandardScaler.
* Tuned the SVM using GridSearchCV and stratified cross-validation.
* Evaluated models using accuracy, balanced accuracy, recall and F1-score.
* Analysed confusion matrices and feature importance.

Model Performance

* Dummy Baseline: Accuracy 86.4%, Balanced Accuracy 50.0%, Good Wine Recall 0.0%, F1-score 0.000
* Random Forest: Accuracy 88.2%, Balanced Accuracy 68.1%, Good Wine Recall 40.5%, F1-score 0.484
* Tuned SVM: Accuracy 79.8%, Balanced Accuracy 79.2%, Good Wine Recall 78.4%, F1-score 0.513

Key Finding

The main takeaway from this project is that the model with the highest overall accuracy is not always the most helpful.

Random Forest achieved the highest accuracy, but it identified only 40.5% of the good wines.

The tuned SVM had lower overall accuracy, but it identified 78.4% of good wines and had the best balanced accuracy.

This shows why recall, F1-score, and balanced accuracy matter when working with imbalanced classification problems.

