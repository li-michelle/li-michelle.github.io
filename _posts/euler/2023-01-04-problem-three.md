---
layout: default
title: "Problem 3"
tags: project-euler
---

**The Problem**
The prime factors of 13195 are 5, 7, 13, and 29. 

What is the largest prime factor of the number 600851475143?

**The Code**

```python 
import math
prime_factors = []
def max_prime(n): 
    while n % 2 == 0:
        prime_factors.append(2)
        n = n / 2
    for i in range(3, (int(math.sqrt(n))+ 1), 2): 
        while n % 1 == 0:
            prime_factors.append(i)
            n = n / i
    print(max(prime_factors))
max _prime(600851475143)
```

**The Thought Process**
Again, an old solution, but one that uses the increment syntax for range(). Uses the logic that the greatest possible prime factor would just be the square root of the number( + 1 for insurance(haha jokes)). 

I used an array because it would just be a lot more memory to check and then update, would make more sense to just store it and then max the array value at the end. 

**The Solution**
6857