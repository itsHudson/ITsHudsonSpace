# 4. DATA COMPONENTS

This section explains the building blocks of machine learning data.

A model learns from data, so if the data is:
- incomplete
- wrong
- messy
- poorly split

The model will perform badly.

Common rule:

**Garbage In → Garbage Out (GIGO)**

Bad data → Bad model predictions

---

## 4.1 Features (X)

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Features (X) | Input variables used by the model to make predictions | Model receives these values and learns patterns | House size, location | Core input of ML |
| Raw Features | Original collected data | Comes directly from source | Customer age | May need cleaning |
| Processed Features | Cleaned/transformed features | Converted into usable format | Encoded gender | Better for training |
| Feature Selection | Choosing useful features | Remove irrelevant variables | Remove customer ID | Improves performance |

---

## 4.2 Labels (Y)

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Labels (Y) | Correct output the model must learn | Model compares prediction with correct answer | House price = RM500,000 | Required in supervised learning |
| Classification Label | Category output | Fixed class label | Spam / Not Spam | Used in classification |
| Regression Label | Numeric output | Continuous value | Salary = RM8,000 | Used in regression |
| Ground Truth | Real correct answer | Used for evaluation | Real diagnosis | Another common term |

---

## 4.3 Dataset

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Dataset | Collection of many data records | Stores features and labels | 10,000 customer records | Foundation of ML |
| Row | One single data record | One observation/example | One customer | Also called sample |
| Column | One variable/feature | Represents one attribute | Age column | Structured data format |
| Structured Dataset | Organized table format | Rows + columns | Excel table | Most common |
| Unstructured Dataset | Non-table format | Text, images, videos | Photos | More complex |

---

## 4.4 Dataset Structure Example

| House Size | Location | Number of Rooms | House Age | Price |
| --- | --- | --- | --- | --- |
| 1000 sqft | Kuala Lumpur | 3 | 5 years | RM500,000 |
| 1200 sqft | Selangor | 4 | 3 years | RM650,000 |

---

## 4.5 Training Set

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Training Set | Data used to train model | Model learns patterns here | 80% of data | Largest dataset split |
| Model Learning | Adjusts weights/parameters | Learns relationships | House pricing | Learning only happens here |
| Repeated Training | Runs many times | Improves model | Multiple epochs | Common process |

---

## 4.6 Validation Set

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Validation Set | Data used during model improvement | Tests model during development | 10% of data | Helps tuning |
| Hyperparameter Tuning | Adjust settings | Find better model settings | Learning rate tuning | Important step |
| Overfitting Detection | Detect memorization | Compare train vs validation performance | Accuracy drop | Helps prevent overfitting |

---

## 4.7 Test Set

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Test Set | Final evaluation dataset | Used after training is complete | 10% of data | Must stay unseen |
| Final Performance Check | Measures true performance | Model predicts on new data | Final accuracy | Real-world simulation |
| No Training Allowed | Never train on test data | Prevent cheating | Hidden exam paper | Very important |

---

## 4.8 Dataset Split

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Dataset Split | Dividing dataset into multiple parts | Separate train/validation/test | 70/15/15 | Standard process |
| Random Shuffle | Mix data before splitting | Prevent bias | Random customer order | Important |
| No Overlap | Same data cannot appear twice | Prevent leakage | Duplicate records | Critical |

---

## 4.8.1 Common Split Ratios

| Training Set | Validation Set | Test Set | Usage | Notes |
| --- | --- | --- | --- | --- |
| 80% | 10% | 10% | Very common | Balanced for large datasets |
| 70% | 15% | 15% | Balanced split | Common choice |
| 60% | 20% | 20% | Small datasets | More evaluation data |

---

## 4.9 Data Leakage

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Data Leakage | Model accidentally learns future/test information | Model gets unfair advantage | Using test data in training | Very dangerous |
| Fake High Accuracy | Results look very good | Model cheats | 99% accuracy | Misleading |
| Real World Failure | Performs badly later | Cannot generalize | Production failure | Must avoid |

---

## 4.10 Feature Quality

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Good Features | Useful input variables | Helps model learn correctly | Salary | Improves accuracy |
| Bad Features | Irrelevant inputs | Confuses model | Random ID | Hurts performance |
| Missing Features | Important variables missing | Weak predictions | Missing credit score | Lower performance |

---

## 4.11 Data Types

| Data Type | Definition | Example | Usage | Notes |
| --- | --- | --- | --- | --- |
| Numerical Data | Number values | Age, salary | Regression/Classification | Very common |
| Categorical Data | Group values | Male/Female | Classification | Often needs encoding |
| Text Data | Written words | Reviews | Natural Language Processing (NLP) | Requires preprocessing |
| Image Data | Pictures | X-ray image | Computer Vision | Large datasets needed |
| Time Series Data | Data over time | Stock prices | Forecasting | Order matters |

---

## 4.12 Data Quality Problems

| Problem | Definition | Example | Impact | Solution |
| --- | --- | --- | --- | --- |
| Missing Values | Empty data | Missing salary | Weak model | Imputation |
| Duplicate Data | Same records repeated | Same customer twice | Bias | Remove duplicates |
| Wrong Labels | Incorrect outputs | Spam marked normal | Wrong learning | Fix labels |
| Noise | Random bad data | Typing errors | Lower accuracy | Data cleaning |

---

## 4.13 Real World Examples

| Industry | Input Features | Label | Goal | Example |
| --- | --- | --- | --- | --- |
| Real Estate | Size, location | House price | Predict price | Property website |
| Healthcare | Age, symptoms | Disease type | Predict illness | Hospital system |

---

## 4.13.1 House Price Dataset Example

| Feature 1 | Feature 2 | Feature 3 | Label | Prediction Goal |
| --- | --- | --- | --- | --- |
| House size | Location | Number of rooms | Price | Predict future house prices |

---

## 4.13.2 Medical Dataset Example

| Feature 1 | Feature 2 | Feature 3 | Label | Prediction Goal |
| --- | --- | --- | --- | --- |
| Age | Blood pressure | Symptoms | Disease type | Predict illness |

---

## 4.14 Why Data Components Matter

| Reason | Explanation | Example | Business Impact | Notes |
| --- | --- | --- | --- | --- |
| Better Features | Better learning | Good house data | Higher accuracy | Very important |
| Proper Splitting | Fair evaluation | Train/Test split | Reliable model | Critical |
| Clean Data | Fewer mistakes | Remove missing values | Better predictions | Required |
| No Leakage | Honest evaluation | Hidden test set | Prevent fake success | Essential |

---

## 4.15 Final Summary

| Question | Answer | Example | Notes | Importance |
| --- | --- | --- | --- | --- |
| What are features? | Input variables | House size | Model input | Very important |
| What are labels? | Correct answers | House price | Model target | Required |
| Why split dataset? | Fair training/testing | 80/10/10 split | Prevent cheating | Critical |
| Why care about data quality? | Better data = better model | Clean dataset | Strong predictions | Foundation of ML |
