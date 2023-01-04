---
layout: default
title: "Problem 4"
tag: project-euler
---

**The Problem**
A palindromic number reads the same both ways. The largest palindrome made from the product of two 2-digit number is 9009 = 91 * 99. 

Find the largest palindrome made from the product of two 3-digit numbers. 

**The Code**

```python 
palindrome_list = []
for a in range(999, 0, -1):
    for b in range(a, 100, -1):
        product = a * b
        if product > 0 and str(product) == str(product)[::-1]:
            palindrome_list.append(product)
max_palindrome = max(palindrome_list)
print(max_palindrome)
```
A fun one, that taught me about nested for loops. 

**The Solution**
906609