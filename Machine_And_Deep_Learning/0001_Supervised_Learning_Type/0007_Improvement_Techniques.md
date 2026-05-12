# 7. IMPROVEMENT TECHNIQUES

This section explains methods used to improve Machine Learning (ML) model performance after the first model is built.

Most first models are not perfect:
- low accuracy
- overfitting
- underfitting
- unstable predictions
- slow training

This section helps answer:

**"How do we improve a weak model and make it more reliable?"**

---

## 7.1 Feature Engineering

**Purpose:** This section explains how to create better input data for the model. Models can only learn from the features they receive, so better features often lead to better predictions.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Feature Engineering | Creating, selecting, and transforming features | Create/remove/transform features | Price per square foot | Improves model quality |
| Feature Creation | Create new useful variables | Combine raw data | Age + income ratio | Adds useful signals |
| Feature Removal | Remove useless variables | Delete irrelevant data | Remove customer ID | Reduces noise |
| Feature Transformation | Change feature format | Convert raw values | Date → month/year | Makes data usable |

---

## 7.2 Feature Scaling

**Purpose:** This section explains how to make feature values similar in size so that one feature does not unfairly dominate another feature.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Feature Scaling | Adjust values into similar ranges | Scale large/small values | Age vs salary | Helps fair learning |
| Why Needed | Prevent large values dominating | Equal importance | Income = 100000 | Important for many models |

---

## 7.3 Normalization

**Purpose:** This section explains one type of feature scaling that converts values into a fixed range, usually between 0 and 1.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Normalization | Scales values between 0 and 1 | Uses min-max scaling | Age → 0.65 | Common scaling method |
| Formula | `(x-min)/(max-min)` | Converts range | 0 to 1 output | Easy interpretation |

---

## 7.4 Standardization

**Purpose:** This section explains another scaling method that converts data into a standard format with mean = 0 and standard deviation = 1.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Standardization | Converts data to mean = 0 and standard deviation = 1 | Centers data | Salary values | Common in ML |
| Formula | `(x-mean)/standard deviation` | Standard scale | Around 0 | Useful for normal distributions |

---

## 7.5 Cross Validation (CV)

**Purpose:** This section explains how to evaluate models more reliably by testing them multiple times on different dataset splits.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Cross Validation (CV) | Evaluates model using multiple splits | Train/test repeatedly | 5-fold CV | More reliable evaluation |
| Goal | Reduce overfitting risk | Better validation | Stable scores | Common technique |

---

## 7.5.1 K-Fold Cross Validation

**Purpose:** This subsection explains the most common type of cross validation.

| Step | Process | Input | Output | Purpose |
| --- | --- | --- | --- | --- |
| 1 | Split dataset | Full dataset | K groups | Create folds |
| 2 | Train model | K-1 groups | Trained model | Learn |
| 3 | Validate model | Remaining group | Validation score | Evaluate |
| 4 | Repeat process | Different folds | Multiple scores | Better reliability |
| 5 | Average scores | All results | Final score | Final evaluation |

---

## 7.6 Hyperparameter Tuning

**Purpose:** This section explains how to find the best model settings to improve performance.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Hyperparameter Tuning | Finding best model settings | Test different settings | Tree depth | Improves performance |
| Examples | Learning rate, batch size | Try multiple values | Neural network tuning | Common task |

---

## 7.7 Grid Search

**Purpose:** This section explains a tuning method that tests every possible parameter combination.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Grid Search | Tests all parameter combinations | Exhaustive search | Tree depth + learning rate | Accurate but slow |
| Best For | Small parameter space | Limited combinations | Small datasets | Computationally expensive |

---

## 7.8 Random Search

**Purpose:** This section explains a faster tuning method that tests random parameter combinations.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Random Search | Tests random parameter combinations | Random sampling | Random tree depth | Faster than grid search |
| Best For | Large parameter space | Many combinations | Deep learning tuning | Saves time |

---

## 7.9 Ensemble Methods

**Purpose:** This section explains how combining multiple models can create a stronger final model.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Ensemble Methods | Combine multiple models | Voting/averaging predictions | Random Forest | Improves accuracy |
| Goal | Reduce single model weakness | Stronger predictions | Fraud detection | Common technique |

---

## 7.10 Bagging

**Purpose:** This section explains an ensemble method that trains models independently.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Bagging | Train models independently | Different random datasets | Random Forest | Reduces variance |
| Full Form | Bootstrap Aggregating | Combine predictions | Tree models | Common interview question |

---

## 7.11 Boosting

**Purpose:** This section explains an ensemble method that trains models sequentially to fix previous errors.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Boosting | Train models sequentially | Fix previous errors | Gradient Boosting | Improves accuracy |
| Goal | Focus on difficult examples | Better performance | XGBoost | Powerful method |

---

## 7.12 Regularization

**Purpose:** This section explains how to reduce model complexity to prevent overfitting.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Regularization | Reduces model complexity | Penalizes large weights | Ridge Regression | Prevents overfitting |
| L1 Regularization | Removes features | Some weights become zero | Lasso | Feature selection |
| L2 Regularization | Shrinks weights | Smaller weights | Ridge | Keeps all features |

---

## 7.13 Early Stopping

**Purpose:** This section explains how to stop training before the model starts overfitting.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Early Stopping | Stops training before overfitting | Monitor validation score | Neural networks | Prevents over-training |
| Trigger | Validation worsens | Stop training | Best epoch | Saves time |

---

## 7.14 Data Augmentation

**Purpose:** This section explains how to create more training data when original data is limited.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Data Augmentation | Create extra training data | Modify existing data | Rotate images | Common in deep learning |
| Goal | Increase dataset size | More training examples | Image recognition | Helps small datasets |

---

## 7.15 Dimensionality Reduction

**Purpose:** This section explains how to reduce unnecessary features while keeping important information.

| Topic | Definition | How It Works | Example | Important Notes |
| --- | --- | --- | --- | --- |
| Dimensionality Reduction | Reduce number of features | Keep important information | Principal Component Analysis (PCA) | Reduces complexity |
| Goal | Faster training | Less noise | Large datasets | Useful for many features |

---

## 7.16 Improvement Technique Selection Guide

**Purpose:** This section helps you choose the correct improvement method based on your model problem.

| Problem | Solution | Example | Why It Helps | Notes |
| --- | --- | --- | --- | --- |
| Overfitting | Regularization | Ridge | Reduces complexity | Common fix |
| Underfitting | Better model | Deeper tree | Learns better | Common fix |
| Poor features | Feature engineering | New variables | Better inputs | Important |
| Unstable results | Cross validation | K-fold | Better evaluation | Reliable |
| Slow tuning | Random search | Random parameters | Saves time | Faster |

---

## 7.17 Real World Example

**Purpose:** This section connects all improvement techniques to a real business scenario.

### House Price Prediction Improvement

| Problem | Solution | Result | Example | Outcome |
| --- | --- | --- | --- | --- |
| Poor features | Feature engineering | Better inputs | Price per sqft | Better accuracy |
| Overfitting | Regularization | Better generalization | Ridge | Stable predictions |
| Weak model | Ensemble method | Stronger predictions | Random Forest | Higher accuracy |

---

## 7.18 Final Summary

**Purpose:** This section summarizes when and why improvement techniques are used.

| Question | Answer | Example | Notes | Importance |
| --- | --- | --- | --- | --- |
| How improve model performance? | Better data + better tuning | House pricing | Continuous process | Very important |
| Why use scaling? | Fair feature comparison | Age vs salary | Important for some models | Common |
| Why use regularization? | Prevent overfitting | Ridge/Lasso | Better generalization | Critical |
| Why use ensemble methods? | Combine strengths | Random Forest | Higher accuracy | Powerful |
