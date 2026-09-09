# Perceptron Trick

Trains a perceptron (line that splits 2 classes) by fixing mistakes, one point at a time.

## Predict
```
z = w·x + b
ŷ = 1 if z ≥ 0 else 0
```

## Update Rule
```
w = w + lr * (y - ŷ) * x
```

## Steps
Random line → pick random point → wrong? nudge weights → repeat → line separates classes.

## Limitation
Only works if data is linearly separable. If not, transform features first (e.g. `x1² + x2²`).

## project2 Perceptron problem 
# Perceptron Problem

Implementation of a Perceptron classifier from scratch, along with a look at its key limitation — it only works when data is **linearly separable**.

## What's Inside
- Perceptron training using the perceptron trick / gradient descent update rule
- Demonstration of the **perceptron problem**: fails on non-linearly separable data (e.g. XOR, circular patterns)
- Fix using feature **transformation** to make data separable

## Update Rule
```
w = w + lr * (y - ŷ) * x
```

## Limitation Solved Here
| Problem | Cause | Fix Used |
|---|---|---|
| Doesn't converge | Data not linearly separable | Transform features (e.g. x1² + x2²) |

## Tech Used
- Python
- NumPy
- Matplotlib (for visualizing decision boundary)


## Key Takeaway
A basic perceptron can only draw a straight line to separate classes. When data isn't linearly separable, transforming the features (or using a multi-layer network) is required.