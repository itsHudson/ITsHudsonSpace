# 2. CLASSIFICATION (PREDICT CATEGORIES / LABELS / DECISIONS)

## 2.1 What is Classification?

**Classification** is a type of **Supervised Learning (SL)** where a machine learns from past labeled data and predicts a **category**, **group**, or **decision** for new data.

The output is **NOT a number** like regression.

The output must be a **fixed label/category**.

---

## Simple Meaning (Very Easy Version)

Classification is like asking:

> "Which group does this belong to?"

The machine looks at input data, learns patterns from old examples, then chooses the correct category.

---

## Real Life Human Example

Imagine a teacher checking exam papers:

Student Score = 95 → Grade A  
Student Score = 70 → Grade B  
Student Score = 40 → Grade C  

Teacher is classifying students into categories.

---

Another example:

Doctor checks patient symptoms:

- Fever
- Cough
- Headache

Doctor decides:

- Flu
- COVID-19
- Normal Cold

This is classification.

---

## Machine Learning Example

Email message:

> "Congratulations! You won $10,000"

Machine checks:

- suspicious words
- links
- sender information

Output:

- Spam
- Not Spam

---

# 2.2 Why Classification is Important?

Many real-world systems need to make decisions.

Businesses usually do not ask:

> "Give me a random number"

They ask:

- Should we approve this loan?
- Is this transaction fraud?
- Is this customer likely to leave?
- Which animal is this?
- Is this disease dangerous?

Classification helps automate these decisions.

---

# 2.3 Input and Output in Classification

| Component | Meaning | Example |
|------------|----------|----------|
| Input Data (X) | Information given to the model | Age, salary, email text |
| Features | Individual pieces of input data | age = 25 |
| Model | Learns patterns from training data | Decision Tree |
| Output Label (Y) | Final predicted category | Approve / Reject |

---

## Example 1: Loan Approval

Input:

- Salary = RM5000
- Credit Score = Good
- Debt = Low

Output:

- Approve Loan

OR

- Reject Loan

---

## Example 2: Animal Classification

Input:

- Has fur
- Four legs
- Barks

Output:

- Dog

---

# 2.4 Full Classification Flow (Step-by-Step)

---

### Step 1: Collect Data

Gather past examples.

Example:

| Email Text | Label |
|-------------|---------|
| Win money now | Spam |
| Meeting at 3PM | Not Spam |

The label tells the machine the correct answer.

---

### Step 2: Clean Data

Remove bad or missing data.

Example:

Wrong email text  
Empty rows  
Duplicate rows

---

### Step 3: Split Data

Usually:

- Training Data = 80%
- Testing Data = 20%

Training data teaches the model.

Testing data checks performance.

---

### Step 4: Train Model

The machine finds patterns.

Example:

Emails with words like:

- Free
- Prize
- Winner

may often be spam.

---

### Step 5: Make Prediction

New email arrives:

> "Claim your free reward"

Model predicts:

Spam

---

### Step 6: Evaluate Performance

Check if model is accurate.

Example:

Out of 100 emails:

Correct = 95  
Wrong = 5  

Accuracy = 95%

---

# 2.5 Mathematical Representation

Input features:

X

Output label:

Y

Goal:

Learn function:

:contentReference[oaicite:0]{index=0}

Meaning:

Machine learns how to convert input data into correct category output.

---

# 2.6 Types of Classification

---

## A. Binary Classification

Only **2 possible outputs**

Examples:

- Yes / No
- True / False
- Spam / Not Spam
- Fraud / Not Fraud
- Pass / Fail

---

### Example

Bank loan system:

Output:

- Approve
- Reject

Only two choices.

---

## B. Multi-Class Classification

More than 2 categories.

Examples:

- Cat
- Dog
- Bird

OR

- Grade A
- Grade B
- Grade C
- Grade D

---

### Example

Handwritten digit recognition:

Output:

0,1,2,3,4,5,6,7,8,9

---

## C. Multi-Label Classification

One input can have multiple labels at the same time.

---

Example:

Photo contains:

- Dog
- Tree
- Car

One image → many labels

---

# 2.7 Common Classification Algorithms

---

## 1. Logistic Regression (LR)

Despite the name "regression", it is used for classification.

Used for:

- Yes/No prediction
- Simple binary problems

Example:

Will customer buy product?

- Yes
- No

---

## 2. Decision Tree (DT)

Makes decisions like asking questions.

Example:

Age > 18?

Yes → Continue  
No → Stop

---

## 3. Random Forest (RF)

Uses many decision trees together.

Final answer comes from majority voting.

Example:

10 trees vote:

7 say Fraud  
3 say Not Fraud

Final output:

Fraud

---

## 4. Support Vector Machine (SVM)

Finds the best boundary between categories.

Example:

Separate cats from dogs.

---

## 5. K-Nearest Neighbors (KNN)

Full form:

K-Nearest Neighbors (KNN)

Looks at nearby similar data points.

Example:

Most nearby fruits are apples → predict apple.

---

## 6. Naive Bayes (NB)

Uses probability.

Often used for text classification.

Example:

Spam detection

---

## 7. Neural Network (NN)

Works well for complex tasks.

Used in:

- Image recognition
- Speech recognition
- Deep learning systems

---

# 2.8 Classification Output

The model may return:

---

## A. Predicted Label

Example:

Spam

---

## B. Probability Score

Example:

Spam = 95%  
Not Spam = 5%

Final answer:

Spam

---

# 2.9 How We Measure Classification Performance

---

## Accuracy

How many predictions are correct?

Formula:

:contentReference[oaicite:1]{index=1}

Example:

90 correct out of 100

Accuracy = 90%

---

## Precision

Out of predicted positives:

How many are truly correct?

Example:

Fraud alerts generated = 20

Actual fraud = 15

Precision = 75%

---

## Recall

Out of actual positives:

How many were found?

Example:

20 fraud cases exist

Model found 18

Recall = 90%

---

## F1 Score

Balances precision and recall.

Useful when classes are imbalanced.

---

## Confusion Matrix

Shows:

- True Positive (TP)
- True Negative (TN)
- False Positive (FP)
- False Negative (FN)

Helps understand mistakes.

---

# 2.10 Real World Use Cases

| Industry | Problem | Output |
|-----------|-----------|----------|
| Banking | Loan approval | Approve / Reject |
| Banking | Fraud detection | Fraud / Not Fraud |
| Healthcare | Disease prediction | Sick / Healthy |
| Email | Spam detection | Spam / Not Spam |
| Shopping | Product recommendation category | Buy / Not Buy |
| Schools | Student grading | Grade A/B/C |

---

# 2.11 Classification vs Regression

| Classification | Regression |
|----------------|-------------|
| Predict category | Predict number |
| Output labels | Output continuous values |
| Spam / Not Spam | House price prediction |
| Cat / Dog | Temperature prediction |

---

## Example

Classification:

"Is this fruit an apple or orange?"

Regression:

"What is the exact weight of this fruit?"

---

# 2.12 Common Problems in Classification

---

## Overfitting

Model memorizes training data too much.

Performs badly on new data.

---

## Underfitting

Model too simple.

Cannot learn patterns properly.

---

## Imbalanced Dataset

One class has too much data.

Example:

99 normal transactions  
1 fraud transaction

Model may struggle.

---

## Noisy Data

Wrong labels

Missing values

Bad quality data

---

# 2.13 Final Full Flow Example

Online shopping fraud detection:

Step 1: Collect old transaction data  
Step 2: Label fraud/not fraud  
Step 3: Train model  
Step 4: Test model  
Step 5: Deploy model  
Step 6: Detect fraud in real time

---

## Final Summary

Classification answers:

> "Which category does this belong to?"

It is used when output must be a fixed decision.

Examples:

- Spam / Not Spam
- Approve / Reject
- Fraud / Not Fraud
- Cat / Dog
- Sick / Healthy

This is one of the most common Machine Learning tasks in real businesses.
