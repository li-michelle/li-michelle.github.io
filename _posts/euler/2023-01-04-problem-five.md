---
layout: default
title: "Problem 5"
tag: project-euler 
--- 
**The Problem**

2520 is the smallest number that can be divided by each of the numbers from 1 to 10 without any remainder.

What is the smallest positive number that is evenly divisible by all of the numbers from 1 to 20?

**The Code**

```python 
n = 2520
count = 0
while count != 20:
  for i in range(1,20):
    if n % i == 0:
      count += 1
    else:
      count = 0 
      n += 1

print(n)
```

**The Thought Process**

The first one I've done after finishing a full year as a mathematics student! Honestly finished this a lot faster than I thought I would, only took me about two tries. However, this method is pretty slow; the first time was taking too long so I changed the starting number. Wondering if there's a way to make this faster...

