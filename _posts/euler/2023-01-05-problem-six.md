---
layout: default
title: "Problem 6"
tag: project-euler
---

**The Problem**

Find the difference between the sum of the squares of the first one hundred natural numbers and the square of the sum.

**The Code**

```python 
first_sum = 0
for i in range(101):
  first_sum += (i * i)

second_sum = 0
for i in range(101):
  second_sum += i

second_sum = second_sum * second_sum 

difference = (second_sum - first_sum)
print(difference)

```

**Thoughts**

This took me an embarassingly long amount of time and I don't want to talk about it(it took a long time because I forgot how for loop ranges work so I wasn't actually adding 100 to any of my sums and I felt very dumb when I discovered. 