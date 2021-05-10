# 10-Days-of-Statistics
Worked Solutions of Hackerrank's 10 Days of Statistics

Day 0: Mean, Median, and Mode Solution
```python
STDIN = input 
from collections import Counter
import pandas as pd 
import numpy as np

n = int(input())
data = sorted([int(i) for i in input().split()]) 
data_s = pd.Series(data)

print(data_s.mean())
print(data_s.median())
print(data_s.mode()[0])
```

```python
STDIN = input 
from collections import Counter
import pandas as pd 
import numpy as np

n = int(input())
data = sorted([int(i) for i in input().split()]) 
data_s = pd.Series(data)

print(data_s.mean())
print(data_s.median())
print(data_s.mode()[0])
```
Day 0: Weighted Mean
Solution

Day 0: Quartiles
Solution

Day 1: Interquartile Range
Solution
