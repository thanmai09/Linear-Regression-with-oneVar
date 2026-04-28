# 📈 Linear Regression with One Variable

A clean Python implementation of **Univariate Linear Regression** from scratch — covering hypothesis function, cost function, and gradient descent — without relying on high-level ML libraries.

---

## 📌 Overview

This project implements Linear Regression with a single feature (one variable) to understand the core mechanics of supervised machine learning. The model learns the best-fit line for a dataset by minimizing the cost function using **Gradient Descent**.

**Hypothesis Function:**

$$h_\theta(x) = \theta_0 + \theta_1 x$$

**Cost Function (Mean Squared Error):**

$$J(\theta_0, \theta_1) = \frac{1}{2m} \sum_{i=1}^{m} \left( h_\theta(x^{(i)}) - y^{(i)} \right)^2$$

---

## 📂 Project Structure
Linear-Regression-with-oneVar/
│
├── data/
│   └── data.txt               # Training dataset (X, y)
│
├── linear_regression.py       # Core implementation
├── gradient_descent.py        # Gradient descent logic
├── cost_function.py           # MSE cost function
├── plot.py                    # Data & regression line visualization
├── main.py                    # Entry point
└── README.md

---

## 🧠 Concepts Covered

- Hypothesis function for linear regression
- Mean Squared Error (MSE) cost function
- Gradient Descent optimization
- Visualization of the regression line
- Convergence of cost over iterations

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.x installed along with the following libraries:

```bash
pip install numpy matplotlib
```

### Clone the Repository

```bash
git clone https://github.com/thanmai09/Linear-Regression-with-oneVar.git
cd Linear-Regression-with-oneVar
```

### Run the Project

```bash
python main.py
```

---

## 📊 Results

The model plots:
- The **training data** as scatter points
- The **best-fit regression line** after gradient descent converges
- The **cost vs. iterations** curve showing the convergence of gradient descent

---

## ⚙️ Parameters

| Parameter        | Description                          | Default |
|-----------------|--------------------------------------|---------|
| `alpha`         | Learning rate                        | `0.01`  |
| `iterations`    | Number of gradient descent steps     | `1500`  |
| `theta_0`       | Initial intercept                    | `0`     |
| `theta_1`       | Initial slope                        | `0`     |

You can tweak these in `main.py` to observe how they affect convergence.

---

## 📐 Algorithm Steps

1. Load and visualize the dataset
2. Initialize parameters θ₀ and θ₁ to zero
3. Compute the cost `J(θ)` using MSE
4. Apply **Gradient Descent** to minimize `J(θ)`:
   - Update θ₀ and θ₁ simultaneously
   - Repeat for `n` iterations
5. Plot the final regression line

---

## 🛠️ Built With

- **Python 3**
- **NumPy** — numerical computations
- **Matplotlib** — data visualization

---

## 📚 References

- [Andrew Ng's Machine Learning Course – Coursera](https://www.coursera.org/learn/machine-learning)
- [Linear Regression – Wikipedia](https://en.wikipedia.org/wiki/Linear_regression)

---

## 🙋‍♀️ Author

**Thanmai** — [@thanmai09](https://github.com/thanmai09)

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).
