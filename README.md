# Day-73--Linear-Regression

###  Overview

**Logistic Regression** is a **supervised machine learning algorithm** used for **classification problems**.

Unlike Linear Regression, it predicts **probabilities** and outputs values between **0 and 1**.

---

##  What is Logistic Regression?

It uses a **sigmoid (logistic) function** to map values into a probability range.

Equation:

```id="h9k3dp"
p = 1 / (1 + e^(-z))
```

Where:

* **p** → probability
* **z** → linear combination of inputs

---

##  Types of Logistic Regression

### 1️ Binary Classification

* Two classes (0 or 1)
  Example: Spam vs Not Spam

### 2️ Multiclass Classification

* More than two classes

---

##  Implementation (Python)

```python id="5b9m2x"
from sklearn.linear_model import LogisticRegression
import numpy as np

X = np.array([[1], [2], [3], [4]])
y = np.array([0, 0, 1, 1])

model = LogisticRegression()
model.fit(X, y)

prediction = model.predict([[2.5]])
print(prediction)
```

---

##  Evaluation Metrics

* **Accuracy**
* **Precision**
* **Recall**
* **Confusion Matrix**

---

##  Use Cases

* Spam detection
* Fraud detection
* Disease prediction
* Customer churn prediction

---

##  Key Takeaways

- Used for classification problems
- Outputs probabilities
- Based on sigmoid function
- Simple and effective model
