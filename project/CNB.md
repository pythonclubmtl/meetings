<!-- $theme: default -->
<!-- footer: #pythonclub - project 01/04/2019 -->
<!-- $size: 16:9 -->


# Project

### Vectorizer / Classifier

1. Build a function that imports the CSV file `pythonclubmtl/learning_python3/datasets/3dprinting-crypto.csv` into 2 lists: `labels` (y) and `documents` (X)
2. Use the `TfidfVectorizer function, followed by `train_test_split` from `scikit-learn` to automatically divide your categories and labels into 3 categories: `X_train`, `y_train`, `X_test` and `y_test` 
3. Train a Complement Multinomial Naive Bayes classifier (`ComplementNB()` from `scikit-learn`) jusing the `X_train` and `y_train` datasets
4. Use the `ComplementNB().predict(X_test)` followed by `ComplementNB().score(X_test, y_test)` to evaluate the performance of your classifier over the test dataset

<!-- *footer: -->

---
