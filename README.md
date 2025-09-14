

# 🚀 Gradient Descent for Linear Regression

##  Student Info

* **Name:** Srinivas Reddy Pittu
* **Student ID:** 700777009
* **Assignment:** Implement Gradient Descent for Linear Regression (without using scikit-learn’s `LinearRegression`)

---

### 📖 Problem Statement

Implement Linear Regression from scratch using both the **Normal Equation** and **Gradient Descent**, train both on the same dataset, and compare their results to evaluate differences in parameters, predictions, and efficiency.

---

### 📊 Dataset

* Generated a dataset of **200 samples**
* $y = 3 + 4x + \epsilon$, where $\epsilon$ is Gaussian noise
* $x \in [0,5]$ uniformly sampled

---

### 🛠️ Implementation

#### 1️⃣ Dataset Generation

* Generated 200 data samples
* Added Gaussian noise to the data
* Visualized the raw dataset with a plot

#### 2️⃣ Closed-Form Solution (Normal Equation)

* Added a bias column of 1’s to $X$
* Calculated model parameters using $\theta = (X^T X)^{-1} X^T y$
* Printed the intercept and slope values
* Plotted the fitted regression line over the raw data

#### 3️⃣ Gradient Descent

* Initialized $\theta = [0,0]$
* Set learning rate $\eta = 0.05$
* Plotted the loss curve (MSE vs. iterations)
* Displayed the final intercept and slope values

#### 4️⃣ Comparison

* Reported parameters obtained from both methods
* Verified convergence between the two approaches

---

### 📈 Results

| Method               | Intercept | Slope  |
| -------------------- | --------- | ------ |
| **Closed-Form**      | 2.8452    | 4.0456 |
| **Gradient Descent** | 2.8452    | 4.0456 |

✅ Both methods converged to **nearly the same solution**.

---

### 📝 Short Explanation

Gradient Descent converges to the same parameters as the closed‑form method; the fitted lines overlap visually.
The MSE curve decreases smoothly and plateaus, indicating stable convergence with (Teta=0.05) over 1000 iterations.
