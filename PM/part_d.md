## 1. Prompt Given to AI

Explain normal distribution, Z-score, and hypothesis testing with a simple Python example.

---

## 2. AI Output (My Notes)

Normal distribution is a bell shaped curve where most values are around mean.

Z-score is used to standardize data using formula (x - mean) / std.

Hypothesis testing is used to make decision using data.

* H0: assumption (mean = value)
* H1: opposite

---

## Code Example

```python
import numpy as np

# generate data

data = np.random.normal(50, 10, 100)

# mean
mean = 0
for x in data:
    mean += x
mean = mean / len(data)

# std
sum_sq = 0
for x in data:
    sum_sq += (x - mean)**2
std = (sum_sq / len(data))**0.5

# z-score for first value
z = (data[0] - mean) / std

print("Mean:", mean)
print("Std:", std)
print("Z-score of first value:", z)
```

---

## 3. Evaluation

### Is explanation correct?

Yes explanation is basic but correct.

* Normal distribution explained correctly
* Z-score formula correct
* Hypothesis testing idea is correct

---

### Is code correct and runnable?

Yes code is working.

* Data generation is correct
* Mean and std calculated properly using loop
* Z-score calculation is correct

---

## Conclusion

Concepts are correct and code is simple and understandable. Good for beginners.
