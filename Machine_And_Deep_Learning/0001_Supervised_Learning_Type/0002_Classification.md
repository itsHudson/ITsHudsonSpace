# 2. CLASSIFICATION (PREDICT CATEGORIES / LABELS / DECISIONS)

---

## 2.1 Definition

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Classification | A type of **Supervised Learning (SL)** that predicts a category, label, or decision instead of a number | The model learns from past labeled data and chooses the correct category for new data | Spam / Not Spam | Output must be a fixed category |
| Main Goal | Identify which group something belongs to | Compare input patterns with learned patterns | Cat / Dog | Used for decision-making problems |
| Output Type | Categorical output | Returns labels/classes | Approve / Reject | Different from regression |

---

## 2.2 Simple Classification Flow

| Step | Process | Input | Output | Purpose |
| --- | --- | --- | --- | --- |
| 1 | Collect Input Data | Email text | Raw email | Provide data to model |
| 2 | Feature Checking | Words, links, sender info | Important patterns | Find useful signals |
| 3 | Pattern Matching | Compare with learned spam patterns | Probability scores | Decide likely category |
| 4 | Final Prediction | Model selects category | Spam | Final classification result |

---

## 2.3 General Formula

| Component | Meaning | Example | Output | Notes |
| --- | --- | --- | --- | --- |
| X | Input Features | Age, salary | Raw data | Information given to model |
| f(X) | Learning Model | Decision Tree | Pattern learning | Model process |
| Y | Output Label | Approve / Reject | Final prediction | Category result |

| Formula | Meaning | Example | Output | Notes |
| --- | --- | --- | --- | --- |
| `f(X) = Y` | Model converts input into category output | Email → Spam | Category | Core idea of classification |

---

## 2.4 Why Classification is Important

| Industry | Problem | Classification Output | Why It Matters | Example |
| --- | --- | --- | --- | --- |
| Banking | Loan approval | Approve / Reject | Faster decisions | Bank loans |
| Banking | Fraud detection | Fraud / Not Fraud | Prevent financial loss | Credit card fraud |
| Healthcare | Disease diagnosis | Sick / Healthy | Faster treatment | Disease prediction |
| Email | Spam filtering | Spam / Not Spam | Cleaner inbox | Gmail spam filter |
| Education | Student grading | Grade A / B / C | Faster grading | School systems |
| Retail | Purchase prediction | Buy / Not Buy | Better marketing | Product recommendations |

---

## 2.5 Input Components

| Component | Definition | Example | Why Important | Notes |
| --- | --- | --- | --- | --- |
| Features | Individual input variables | Age | Helps model learn patterns | Also called variables |
| Dataset | Collection of training data | Customer records | Needed for training | Large datasets improve learning |
| Labels | Correct answers | Spam | Teach model correct output | Required in supervised learning |
| Training Data | Data used for learning | Past fraud records | Helps model learn | Usually largest portion |
| Testing Data | Data used for evaluation | New fraud records | Measures performance | Usually smaller portion |

---

## 2.6 Types of Classification

| Type | Definition | Number of Outputs | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Binary Classification | Predicts one of two classes | 2 | Yes / No | Most common beginner example |
| Multi-Class Classification | Predicts one class from many classes | More than 2 | Cat / Dog / Bird | Only one final output |
| Multi-Label Classification | Predicts multiple labels at once | Multiple outputs | Dog + Tree + Car | One input can have many labels |

---

## 2.7 Full Classification Workflow

| Step | Process | Input | Output | Purpose |
| --- | --- | --- | --- | --- |
| 1 | Data Collection | Raw business data | Dataset | Gather information |
| 2 | Data Cleaning | Raw dataset | Clean dataset | Remove errors |
| 3 | Data Splitting | Clean dataset | Training/Test sets | Fair evaluation |
| 4 | Model Training | Training data | Trained model | Learn patterns |
| 5 | Model Testing | Testing data | Accuracy results | Measure performance |
| 6 | Prediction | New unseen data | Predicted label | Real-world usage |
| 7 | Improvement | Weak model | Better model | Improve performance |
| 8 | Deployment | Final model | Real system | Business usage |

---

## 2.8 Common Classification Algorithms

| Algorithm | Full Form | How It Works | Example | Limitation |
| --- | --- | --- | --- | --- |
| Logistic Regression (LR) | Logistic Regression | Uses probability to predict categories | Loan approval | Struggles with complex patterns |
| Decision Tree (DT) | Decision Tree | Uses rule-based splitting | Student pass/fail | Can overfit |
| Random Forest (RF) | Random Forest | Combines multiple trees | Fraud detection | Slower than single tree |
| Support Vector Machine (SVM) | Support Vector Machine | Finds best separation boundary | Image classification | Hard with huge datasets |
| K-Nearest Neighbors (KNN) | K-Nearest Neighbors | Looks at nearest similar data | Fruit classification | Slow with large datasets |
| Naive Bayes (NB) | Naive Bayes | Uses probability rules | Spam detection | Assumes feature independence |
| Neural Network (NN) | Neural Network | Learns complex patterns using layers | Face recognition | Requires large datasets |

---

## 2.9 Model Output Types

| Output Type | Definition | Example | Why Useful | Notes |
| --- | --- | --- | --- | --- |
| Predicted Label | Final selected category | Spam | Easy decision-making | Most common output |
| Probability Score | Confidence percentage | Spam = 95% | Shows confidence level | Common in finance/healthcare |
| Ranking Output | Sorts possible classes | Product recommendation | Better recommendations | Less common |

---

## 2.10 Evaluation Metrics

| Metric | Formula | What It Measures | Example | When to Use |
| --- | --- | --- | --- | --- |
| Accuracy | Correct Predictions / Total Predictions | Overall correctness | 95 correct out of 100 | Balanced datasets |
| Precision | True Positive / (True Positive + False Positive) | Correct positive predictions | Fraud alerts | False alarms are costly |
| Recall | True Positive / (True Positive + False Negative) | Finds actual positives | Disease detection | Missing cases is dangerous |
| F1 Score | Balance of Precision + Recall | Balances both metrics | Fraud detection | Imbalanced datasets |
| Confusion Matrix | Table of prediction results | Shows mistakes | TP/TN/FP/FN | Error analysis |

---

## 2.11 Confusion Matrix Terms

| Term | Full Form | Meaning | Example | Notes |
| --- | --- | --- | --- | --- |
| TP | True Positive | Correct positive prediction | Fraud predicted as fraud | Good prediction |
| TN | True Negative | Correct negative prediction | Normal predicted as normal | Good prediction |
| FP | False Positive | Wrong positive prediction | Normal predicted as fraud | False alarm |
| FN | False Negative | Wrong negative prediction | Fraud predicted as normal | Dangerous mistake |

---

## 2.12 Common Problems in Classification

| Problem | Definition | Cause | Example | Solution |
| --- | --- | --- | --- | --- |
| Overfitting | Model memorizes training data too much | Model too complex | High train accuracy, low test accuracy | Regularization |
| Underfitting | Model too simple | Weak learning | Poor predictions | Use better model |
| Imbalanced Dataset | One class dominates | Unequal data distribution | 99 normal, 1 fraud | Resampling |
| Noisy Data | Poor quality data | Wrong labels | Incorrect training examples | Data cleaning |

---

## 2.13 Classification vs Regression

| Feature | Classification | Regression | Similarity | Example |
| --- | --- | --- | --- | --- |
| Output | Category | Number | Both are supervised learning | Spam vs house price |
| Goal | Choose class | Predict value | Learn patterns | Fraud vs temperature |
| Result Type | Fixed labels | Continuous values | Use training data | Approve vs salary |

---

## 2.14 Real World Applications

| Industry | Input | Model Task | Output | Example |
| --- | --- | --- | --- | --- |
| Banking | Credit score | Loan approval | Approve / Reject | Loan system |
| Healthcare | Symptoms | Disease prediction | Sick / Healthy | Hospital AI |
| Retail | Customer behavior | Purchase prediction | Buy / Not Buy | E-commerce |
| Security | Face image | Face recognition | Person identity | Phone unlock |
| Email | Email text | Spam detection | Spam / Not Spam | Gmail |

---

## 2.15 End-to-End Example (Fraud Detection System)

| Step | Input | Process | Output | Purpose |
| --- | --- | --- | --- | --- |
| 1 | Transaction records | Collect historical data | Dataset | Prepare training data |
| 2 | Fraud labels | Label transactions | Labeled dataset | Teach model |
| 3 | Training data | Train model | Trained classifier | Learn fraud patterns |
| 4 | Testing data | Evaluate model | Performance score | Check model quality |
| 5 | New transaction | Predict fraud | Fraud / Not Fraud | Real-time decision |

---

## 2.16 Final Summary

| Question | Answer | Example | Notes | Importance |
| --- | --- | --- | --- | --- |
| What does classification do? | Predict categories | Spam detection | Most common ML task | Very important |
| What output does it give? | Labels | Yes / No | Not numbers | Key difference |
| When should it be used? | Fixed decisions | Loan approval | Binary/Multi-class | Common in business |
| Why learn it? | Many real systems use it | Fraud detection | Foundation topic | Required in ML |
