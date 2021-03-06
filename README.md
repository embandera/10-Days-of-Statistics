# 10-Days-of-Statistics-Python
Worked Solutions of Hackerrank's 10 Days of Statistics
- Day 0: Mean, Median, and Mode Solution
- Day 0: Weighted Mean
- Day 0: Quartiles
- Day 1: Interquartile Range

# Day 0: Mean, Median, and Mode Solution
```python
STDIN = input 
from collections import Counter
import pandas as pd 

n = int(input())
data = sorted([int(i) for i in input().split()]) 
data_s = pd.Series(data)

print(data_s.mean())
print(data_s.median())
print(data_s.mode()[0])
```
v.2
```python
from collections import Counter
n = int(input())
x = sorted(list(map(int, input().split())))

# mean
mean = sum(x) / n

# median
if n % 2 == 1:
    index = n // 2
    median = x[index]
else:
    ind = n // 2
    median = (x[ind-1] + x[ind]) / 2

# mode
counter = Counter(x)
most_common = counter.most_common()
mode = most_common[0]
print("{:.1f}".format(mean), median, mode[0], sep="\n")
```
Day 0: Weighted Mean
Solution

``` python 
def weightedMean(X, W):
    sum_of_weighted_grades = 0
    
    for i in range(n):
        sum_of_weighted_grades += X[i]*W[i]  
            
    weighted_average = sum_of_weighted_grades / sum(W)
    
    return "{:.1f}".format(weighted_average)
      
    

if __name__ == '__main__':
    n = int(input().strip())

    vals = [int(i) for i in input().rstrip().split()]

    weights = [int(i) for i in input().rstrip().split()]
    
    print(weightedMean(vals, weights))
```

Day 0: Quartiles
Solution

Day 1: Interquartile Range
Solution

Day 1: Standard Deviation
