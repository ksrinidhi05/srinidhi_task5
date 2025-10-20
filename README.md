# Consumer Complaint Text Classification System

This project is a **complete pipeline** for classifying consumer complaints into four categories:

1. Credit Reporting  
2. Debt Collection  
3. Consumer Loan  
4. Mortgage  

It includes **data analysis, preprocessing, feature engineering, model training, evaluation, and prediction**.

---

## Features

- Exploratory Data Analysis (EDA) with visualizations
- Text preprocessing (cleaning, tokenization, lemmatization)
- Feature engineering (word count, character count, stopwords, etc.)
- Multiple machine learning models:
  - Naive Bayes
  - Logistic Regression
  - Linear SVM
  - Random Forest
  - XGBoost
- Model comparison and evaluation with metrics like accuracy, F1-score, precision, recall
- Confusion matrix visualization
- Prediction system for new complaints

---

## Requirements

- Python 3.8+
- Libraries:
  ```bash
  pandas
  numpy
  matplotlib
  seaborn
  wordcloud
  nltk
  scikit-learn
  xgboost

## OUTPUTS:
<img width="1289" height="624" alt="image" src="https://github.com/user-attachments/assets/f0025121-0f9a-4b4d-a3de-d4cfb8f7efd3" />
<img width="1248" height="612" alt="image" src="https://github.com/user-attachments/assets/895c94ed-cb05-44bd-a41b-c0f1d51da659" />
<img width="1170" height="630" alt="image" src="https://github.com/user-attachments/assets/b464c43c-c528-4906-92b9-b938ee29eda7" />
================================================================================
CONSUMER COMPLAINT TEXT CLASSIFICATION SYSTEM
================================================================================

[STEP 1/6] Exploratory Data Analysis and Feature Engineering
================================================================================
INITIAL DATA EXPLORATION
================================================================================

Dataset Shape: (11535877, 18)

Column Names:
['Date received', 'Product', 'Sub-product', 'Issue', 'Sub-issue', 'Consumer complaint narrative', 'Company public response', 'Company', 'State', 'ZIP code', 'Tags', 'Consumer consent provided?', 'Submitted via', 'Date sent to company', 'Company response to consumer', 'Timely response?', 'Consumer disputed?', 'Complaint ID']

First Few Rows:
  Date received                                            Product       Sub-product  ... Timely response? Consumer disputed? Complaint ID
0    2020-07-06  Credit reporting, credit repair services, or o...  Credit reporting  ...              Yes                NaN      3730948
1    2025-10-14  Credit reporting or other personal consumer re...  Credit reporting  ...              Yes                NaN     16558024
2    2025-10-10  Credit reporting or other personal consumer re...  Credit reporting  ...              Yes                NaN     16507707
3    2025-10-15  Credit reporting or other personal consumer re...  Credit reporting  ...              Yes                NaN     16593757
4    2025-10-17  Credit reporting or other personal consumer re...  Credit reporting  ...              Yes                NaN     16649455

[5 rows x 18 columns]

Data Types:
Date received                   object
Product                         object
Sub-product                     object
Issue                           object
Sub-issue                       object
Consumer complaint narrative    object
Company public response         object
Company                         object
State                           object
ZIP code                        object
Tags                            object
Consumer consent provided?      object
Submitted via                   object
Date sent to company            object
Company response to consumer    object
Timely response?                object
Consumer disputed?              object
Complaint ID                     int64
dtype: object

Missing Values:
Date received                          0
Product                                0
Sub-product                       235295
Issue                                  6
Sub-issue                         862002
Consumer complaint narrative     8119132
Company public response          5717955
Company                                0
State                              56866
ZIP code                           30229
Tags                            10863856
Consumer consent provided?       1936609
Submitted via                          0
Date sent to company                   0
Company response to consumer          20
Timely response?                       0
Consumer disputed?              10767593
Complaint ID                           0
dtype: int64

================================================================================
FILTERING CATEGORIES
================================================================================

Filtered Dataset Shape: (3521673, 19)

Category Distribution:
0    2163850
1     896044
3     430205
2      31574
Name: Category, dtype: int64

================================================================================
EXPLORATORY DATA ANALYSIS
================================================================================

✓ Category distribution plot saved

Text Length Statistics:
count    3.521673e+06
mean     3.705166e+02
std      9.132358e+02
min      3.000000e+00
25%      3.000000e+00
50%      3.000000e+00
75%      4.280000e+02
max      3.261600e+04
Name: text_length, dtype: float64

Word Count Statistics:
count    3.521673e+06
mean     6.599077e+01
std      1.596810e+02
min      1.000000e+00
25%      1.000000e+00
50%      1.000000e+00
25%      1.000000e+00
50%      1.000000e+00
75%      7.700000e+01
max      6.095000e+03
Name: word_count, dtype: float64
✓ Word count distribution plot saved

================================================================================
GENERATING WORD CLOUDS
================================================================================
✓ Word clouds saved

================================================================================
FEATURE ENGINEERING
25%      1.000000e+00
50%      1.000000e+00
75%      7.700000e+01
max      6.095000e+03
Name: word_count, dtype: float64
✓ Word count distribution plot saved
25%      1.000000e+00
50%      1.000000e+00
75%      7.700000e+01
max      6.095000e+03
50%      1.000000e+00
75%      7.700000e+01
max      6.095000e+03
Name: word_count, dtype: float64
✓ Word count distribution plot saved

================================================================================
GENERATING WORD CLOUDS
================================================================================
✓ Word clouds saved

================================================================================
FEATURE ENGINEERING
================================================================================
✓ Word clouds saved

================================================================================
FEATURE ENGINEERING
================================================================================




















✓ Word clouds saved

================================================================================
FEATURE ENGINEERING
================================================================================




================================================================================
FEATURE ENGINEERING
================================================================================
================================================================================






