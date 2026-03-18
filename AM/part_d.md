# Part D 

## 1. Prompt Given to AI

Explain Python dunder methods with examples for beginners and include a custom class implementation.

---

## 2. AI Output (My Notes)

Dunder methods are special methods in python which have double underscore like **init**, **str** etc.

These methods run automatically when we do some operation.

### Some examples:

* **init** → used when object is created
* **str** → used when we print object
* **add** → used when we use + operator

---

## Code Example

```python
class Book:
    
    def __init__(self, title, price):
        self.title = title
        self.price = price
    
    def __str__(self):
        return "Book: " + self.title + ", Price: " + str(self.price)
    
    def __add__(self, other):
        return self.price + other.price

b1 = Book("Python", 500)
b2 = Book("Data Science", 700)

print(b1)
print("Total:", b1 + b2)
```

### Output:

```
Book: Python, Price: 500
Total: 1200
```

---

## 3. Evaluation

### Are examples correct?

Yes mostly correct.

* **init** working fine
* **str** printing properly
* **add** also giving correct output

---

### Is class working?

Yes class is working.
Output is coming correct and no error.

---

## Conclusion

Dunder methods are useful to make class better. It helps in printing, adding objects etc. It is important concept in python OOP.
