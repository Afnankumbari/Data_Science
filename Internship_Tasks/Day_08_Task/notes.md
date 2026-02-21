
---

# 📘 DAY 8 – NUMPY COMPLETE NOTES 

---

# 🔷 1️⃣ What is NumPy?

**NumPy** stands for:

> **Numerical Python**

It is a powerful Python library used for:

* Mathematical calculations
* Numerical computations
* Scientific computing
* Machine learning operations
* Linear algebra
* Statistical operations

---

# 🔷 2️⃣ Why Do We Need NumPy?

Normal Python lists:

```python
x = ["hello", 1, "data"]
```

Problems:

* Mixed data types
* Slow for large data
* Not optimized for mathematical operations
* No vectorized operations

---



<img width="1024" height="1536" alt="ChatGPT Image Feb 21, 2026, 09_48_05 PM" src="https://github.com/user-attachments/assets/076eebe3-a046-465b-b8c2-b28fe5263851" />

---

# 🔷 3️⃣ Why is NumPy Faster Than Python Lists?

NumPy is faster because:

### ✅ 1. Written in C

* Core implementation is in C language
* C is much faster than Python

### ✅ 2. Contiguous Memory Allocation

* Data stored in continuous memory block
* Faster access
* Better CPU cache usage

### ✅ 3. Homogeneous Data Type

* All elements same type
* No type checking for each element
* Faster computation

### ✅ 4. Vectorization

* No need to use loops
* Performs operation on entire array at once

Example:

```python
array1 = np.array([10000,40000,55000])
array1 + 5000
```

Output:

```
[15000 45000 60000]
```

No loop required!

---

# 🔷 4️⃣ What is ndarray?

NumPy provides a special data structure:

> **ndarray (N-dimensional array)**

This is:

* Faster
* Memory efficient
* Supports multi-dimensional data

---

# 🔷 5️⃣ Creating NumPy Arrays

### Install:

```
pip install numpy
```

### Import:

```python
import numpy as np
```

---

## 1D Array

```python
x = np.array([1,2,3,4])
```

---

## 2D Array

```python
y = np.array([[1,2,3],[4,5,6]])
```

---

## 0D Array (Scalar)

```python
a = np.array(89)
```

---

# 🔷 6️⃣ Important Properties of NumPy Arrays

Let’s say:

```python
x = np.array([1,2,3,4])
```

### ✅ 1. dtype

Tells data type.

```python
x.dtype
```

Output:

```
int32
```

---

### ✅ 2. ndim

Number of dimensions.

* 0D → scalar
* 1D → vector
* 2D → matrix

```python
x.ndim
```

---

### ✅ 3. shape

Tells size in each dimension.

Example:

```python
y = np.array([[1,2,3],[4,5,6]])
y.shape
```

Output:

```
(2,3)
```

Meaning:
2 rows, 3 columns

---

### ✅ 4. size

Total number of elements.

```python
y.size
```

---

# 🔷 7️⃣ Indexing in NumPy

## 1D Array Indexing

```python
x = np.array([10,20,30,40])
x[0]  → 10
x[1]  → 20
```

---

## 2D Array Indexing

```python
y[2,3]
```

Means:

* Row index 2
* Column index 3

---

# 🔷 8️⃣ Slicing in NumPy

## 1D Slicing

```python
x[3:8]
x[:5]
x[1:]
```

Format:

```
array[start:end]
```

---

## 2D Slicing

```python
y[0:3, 0:2]
```

Meaning:

* Rows from 0 to 2
* Columns from 0 to 1

Example Output:

```
[[1,2],
 [5,6],
 [9,10]]
```

---

# 🔷 9️⃣ Statistical Operations

Given:

```python
a = np.array([...])
```

### ✅ Mean

```python
a.mean()
```

### ✅ Sum

```python
a.sum()
```

### ✅ Standard Deviation

```python
a.std()
```

### ✅ Variance

```python
a.var()
```

### ✅ Minimum

```python
a.min()
```

### ✅ Maximum

```python
a.max()
```

---

# 🔷 🔟 Matrix Operations

### Transpose

```python
a.T
```

Rows become columns.

---

# 🔷 1️⃣1️⃣ Vectorization

Vectorization means:

> Performing operations on entire array without loops.

Example:

```python
arr = np.random.rand(1_000_000)
np.sqrt(arr)
```

NumPy computes square root for 1 million values instantly.

Why important?

* Avoid loops
* Faster execution
* Clean code
* Industry standard

---

# 🔷 1️⃣2️⃣ Broadcasting

Broadcasting means:

> Performing operations between arrays of different shapes automatically.

Example:

```python
array1 = np.array([10000,40000,55000])
array1 + 5000
```

Scalar 5000 automatically applied to all elements.

---

# 🔷 1️⃣3️⃣ Linear Algebra Support

NumPy supports:

* Matrix multiplication
* Dot product
* Inverse
* Determinant
* Eigenvalues

Used in:

* ML algorithms
* Neural networks
* Data transformations

---

# 🔷 1️⃣4️⃣ Mathematical Functions

NumPy supports:

```python
np.sin(x)
np.sqrt(x)
np.exp(x)
np.log(x)
```

Used in:

* Deep learning
* Scientific simulation
* Signal processing

---

# 🔷 1️⃣5️⃣ Why NumPy is Important in Industry?

### Used in:

* Machine Learning
* Deep Learning
* AI
* Data Science
* Finance
* Healthcare
* Computer Vision
* Scientific research

---

# 🔷 1️⃣6️⃣ Integration with ML

Important ML libraries depend on NumPy:

* TensorFlow
* PyTorch
* Scikit-learn
* Pandas

Why?

Because:

* ML models work on matrices
* Data is numeric
* Fast computation required

---

# 🔷 1️⃣7️⃣ Advantages of NumPy

1. Fast computation
2. Memory efficient
3. Supports large datasets
4. Vectorized operations
5. Broadcasting
6. Linear algebra support
7. Statistical functions
8. Backbone of ML libraries

---

# 🔷 1️⃣8️⃣ Real Industry Use Cases

NumPy used for:

* ML model training
* Signal processing
* Scientific simulations
* Financial analysis
* Data transformation

---

# 🔷 1️⃣9️⃣ Difference: Python List vs NumPy Array

| Feature       | Python List | NumPy      |
| ------------- | ----------- | ---------- |
| Speed         | Slow        | Fast       |
| Data Type     | Mixed       | Same       |
| Memory        | Scattered   | Contiguous |
| Vectorization | No          | Yes        |
| Used in ML    | No          | Yes        |

---

# 🔷 2️⃣0️⃣ Most Important Interview Questions

### ❓ Why is NumPy faster?

Because:

* Written in C
* Contiguous memory
* Homogeneous data
* Vectorization

### ❓ What is broadcasting?

Automatic expansion of smaller array to match larger array.

### ❓ What is vectorization?

Performing operations on whole array without loops.

---

# 🎯 Final Understanding

NumPy is:

> The foundation of Data Science & Machine Learning.

Without NumPy:

* No fast computation
* No matrix operations
* No ML frameworks
* No large-scale data processing

---

