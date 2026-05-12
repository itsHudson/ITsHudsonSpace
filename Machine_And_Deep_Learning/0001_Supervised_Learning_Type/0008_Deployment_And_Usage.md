# 8. DEPLOYMENT & USAGE

This section explains how Machine Learning (ML) models are used in real-world systems.

Building a model is not the final goal.

A model only becomes valuable when real users, businesses, or systems can actually use it.

This section answers:

```text
"How does a trained model become a real product?"
```

Common real-world goals:

- Deploy model to production
- Make predictions for users
- Handle large traffic
- Monitor performance
- Update model over time

---

# 8.1 Deployment Examples Used Throughout This Section

This section introduces examples reused throughout this topic.

| Example | ML Task | Deployment Type | Real Use Case | Output |
| --- | --- | --- | --- | --- |
| Spam Detection | Classification | Real-time | Gmail | Spam/Not Spam |
| House Price Prediction | Regression | Batch prediction | Property platform | House price |
| Fraud Detection | Classification | Real-time | Banking | Fraud alert |
| Product Recommendation | Recommendation | Large-scale system | E-commerce | Product suggestions |

---

# 8.2 Model Deployment

This section explains how a trained model becomes usable in real systems.

Deployment means moving a trained model into production.

---

## 8.2.1 Deployment Flow

```text
Train model
→ Finalize model
→ Save model
→ Deploy model
→ Receive user input
→ Make predictions
→ Return output
```

---

## 8.2.2 Example A: Spam Detection Deployment (Detailed)

```text
1. Company trains spam model

2. Model learns:
   Spam vs Not Spam

3. Model deployed into email system

4. New email arrives:
   "Win free money now"

5. Model predicts:
   Spam

6. Email moves to spam folder
```

---

## 8.2.3 Example B: House Price Deployment (Detailed)

```text
1. Property company trains house pricing model

2. Model deployed to website

3. User enters:
   - Location
   - House size
   - Bedrooms

4. Model predicts:
   RM850,000

5. Price shown to user
```

---

# 8.3 Model Saving

This section explains storing trained models.

Without saving, retraining would be required every time.

---

## 8.3.1 Common Saving Methods

| Method | File Type | Example | Use Case | Notes |
| --- | --- | --- | --- | --- |
| Pickle | `.pkl` | Scikit-learn model | Python ML | Common |
| Joblib | `.joblib` | Large models | Faster loading | Popular |
| TensorFlow SavedModel | Folder format | Deep learning | TensorFlow | Standard |
| PyTorch Model | `.pt` / `.pth` | Neural networks | PyTorch | Common |

---

## 8.3.2 Example A: Saving Model (Detailed)

```text
1. Train house price model

2. Save model:
house_model.pkl

3. Store model file

4. Reuse later without retraining
```

---

# 8.4 Model Loading

This section explains restoring saved models.

---

## 8.4.1 Example A: Loading Model (Detailed)

```text
1. User visits website

2. System loads:
house_model.pkl

3. Model becomes ready

4. Prediction request begins
```

---

# 8.5 Batch Prediction

This section explains predicting many records at once.

Used when instant response is not needed.

---

## 8.5.1 Batch Prediction Flow

```text
Collect large dataset
→ Send to model
→ Process all records
→ Return predictions
```

---

## 8.5.2 Example A: House Batch Prediction (Detailed)

```text
1. Property company has:
10,000 houses

2. System runs overnight

3. Model predicts prices for all houses

4. Database updates all prices
```

---

## 8.5.3 Example B: Marketing Prediction

```text
1. Company has:
1 million customers

2. Predict who may buy products

3. Send marketing campaigns next day
```

---

# 8.6 Real-Time Prediction

This section explains instant prediction systems.

Predictions must happen immediately.

---

## 8.6.1 Real-Time Flow

```text
User input
→ Model prediction
→ Immediate output
```

---

## 8.6.2 Example A: Fraud Detection (Detailed)

```text
1. Customer swipes credit card

2. Transaction sent to fraud model

3. Model predicts:
Fraud risk = High

4. Bank blocks transaction instantly
```

---

## 8.6.3 Example B: Face Unlock

```text
1. User scans face

2. Model compares face

3. Prediction:
Owner verified

4. Phone unlocks instantly
```

---

# 8.7 API (Application Programming Interface)

This section explains how applications communicate with models.

APIs connect frontend systems to ML models.

---

## 8.7.1 API Flow

```text
Frontend App
→ API Request
→ Model
→ Prediction
→ API Response
→ User
```

---

## 8.7.2 Example A: House Price API (Detailed)

```text
1. User fills website form

2. Website sends API request

3. API sends data to model

4. Model predicts:
RM900,000

5. API returns result to website
```

---

# 8.8 Monitoring

This section explains tracking deployed model performance.

Models may degrade over time.

---

## 8.8.1 Monitoring Tasks

| Task | Purpose | Example | Risk If Ignored | Importance |
| --- | --- | --- | --- | --- |
| Track accuracy | Detect issues | Fraud model | Wrong predictions | High |
| Log failures | Debug issues | API errors | System crashes | High |
| Monitor latency | Check speed | Slow predictions | Bad UX | High |

---

## 8.8.2 Example A: Fraud Monitoring (Detailed)

```text
Before:
95% fraud accuracy

After 6 months:
80%

Problem detected:
Model performance dropping
```

---

# 8.9 Model Drift

This section explains performance decline caused by changing data.

Real-world data changes over time.

---

## 8.9.1 Example A: Customer Behavior Drift (Detailed)

```text
Old shopping behavior:
Offline shopping

New behavior:
Online shopping

Model trained on old data fails
```

---

## 8.9.2 Example B: Fraud Drift

```text
Fraudsters change attack methods

Old fraud patterns become outdated
```

---

# 8.10 Retraining

This section explains updating old models.

---

## 8.10.1 Retraining Flow

```text
Collect new data
→ Add labels
→ Retrain model
→ Test model
→ Deploy updated model
```

---

## 8.10.2 Example A: Recommendation Retraining

```text
Monthly retraining:

Collect new customer behavior

Train updated recommendation model

Deploy improved version
```

---

# 8.11 Versioning

This section explains tracking model versions.

Multiple versions help manage risk.

---

## 8.11.1 Version Tracking Table

| Version | Accuracy | Changes | Status | Notes |
| --- | --- | --- | --- | --- |
| v1 | 85% | Initial model | Old | Baseline |
| v2 | 90% | Better features | Active | Improved |
| v3 | 92% | Better tuning | Testing | New |

---

## 8.11.2 Example A: Rollback Scenario

```text
Version v3 fails in production

Company rolls back to v2
```

---

# 8.12 Pipeline

This section explains automated workflows.

Pipelines automate end-to-end ML systems.

---

## 8.12.1 Pipeline Flow

```text
Collect Data
→ Clean Data
→ Feature Engineering
→ Prediction
→ Store Results
→ Show Output
```

---

## 8.12.2 Example A: E-commerce Pipeline

```text
Customer visits website

System collects behavior

Recommendation model predicts products

Products displayed instantly
```

---

# 8.13 Latency

This section explains prediction speed.

Latency = how fast predictions return.

---

## 8.13.1 Example A: Fraud Latency (Detailed)

```text
Customer swipes card

Prediction takes:
10 seconds

Problem:
Too slow

Transaction already completed
```

---

## 8.13.2 Example B: Good Latency

```text
Prediction time:
50 milliseconds

Fast enough for fraud prevention
```

---

# 8.14 Scalability

This section explains handling large traffic.

Systems must support growing users/data.

---

## 8.14.1 Example A: E-commerce Scaling

```text
Normal traffic:
10,000 users/day

Holiday traffic:
1 million users/day

System scales servers

Predictions continue working
```

---

## 8.14.2 Example B: Streaming Platform

```text
Millions of recommendation requests

System must scale globally
```

---

# 8.15 End-to-End Deployment Example: Fraud Detection System

This section connects everything.

| Step | Input | Process | Output | Purpose |
| --- | --- | --- | --- | --- |
| 1 | Transaction data | Train model | Fraud model | Build |
| 2 | Save model | Store model | File | Deployment prep |
| 3 | Deploy API | Connect banking system | Live model | Real usage |
| 4 | Real-time prediction | Detect fraud | Block transaction | Protect users |
| 5 | Monitor model | Track accuracy | Alerts | Maintain quality |
| 6 | Retrain | Update model | Better model | Long-term performance |

---

## 8.15.1 Full Production Flow

```text
Train
→ Save
→ Deploy
→ Predict
→ Monitor
→ Detect Drift
→ Retrain
→ Redeploy
```

---

# 8.16 Why Deployment Matters

This section explains why deployment is critical.

| Reason | Example | Business Impact | Result | Importance |
| --- | --- | --- | --- | --- |
| Real-world value | Spam filter | Better email experience | Useful product | High |
| Business automation | Fraud detection | Reduce losses | Faster decisions | High |
| Scalability | Recommendations | Serve millions | Growth | High |

---

# 8.17 Final Summary

This section summarizes deployment.

```text
Training Model ≠ Final Goal
```

Real value happens when models are used by real users.

Full lifecycle:

```text
Train Model
→ Deploy Model
→ Serve Predictions
→ Monitor Performance
→ Retrain Model
→ Improve System
```

