# 📄 minOperations

A Python function that calculates the minimum number of operations needed to generate exactly `n` characters using only two actions: **Copy All** and **Paste**.

## 🧠 Problem Description

Starting with one character `'H'`, you can perform two operations:

- **Copy All**: Copies all current characters.
- **Paste**: Pastes the copied characters.

The goal is to reach exactly `n` `'H'` characters using the fewest possible steps.

## 🚀 Function Signature

```python
def minOperations(n: int) -> int
```

- **Parameters**: `n` (int) — Target number of characters.
- **Returns**: Minimum number of operations (int). Returns `0` if `n <= 1`.

## 📌 Approach

This solution uses **prime factorization** to determine the optimal sequence of operations. Each factor represents a sequence of copy-paste steps that builds up the total count efficiently.

## ✅ Examples

```python
minOperations(4)   # ➞ 4
minOperations(9)   # ➞ 6
minOperations(1)   # ➞ 0
```

## 📂 File Structure

```
min_operations/
├── min_operations.py   # Contains the minOperations function
├── README.md           # Project documentation
```

## 🛠️ How to Run

```bash
python3 min_operations.py
```

Or import the function into another script:

```python
from min_operations import minOperations
```
