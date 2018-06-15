```python
from aide_design.play import*
from aide_design.physchem import*
import math

def squared(N):
    for i in range(0,N):
        squared=i**2
        i=i+1
        print(squared)
squared(9)

  def leapyear(year):
      ##1900 to 10^5
      return ((float.is_integer(year/4) or (float.is_integer(year/100)==True and float.is_integer(year/400)==True)) and not (float.is_integer(year/100)==True and float.is_integer(year/400)==False))

def count(N):
  a=[]
  for i in range(1,N+1):
    a.append(i)
    i=i+1
  print((*a), sep='')
  return


def stringConstruction(s):
    list=[]
    for i in range(0,len(s)):
          list.append(s[i])
    print(len(set(list)))
    return
stringConstruction('abcd')

def sumarray(ar):
  n = int(input())
  nums = list(map(int, input().split()))
  sum = 0
  for num in nums:
    sum += num
  print(sum)

def weighted_mean(N,X,Weight):
  Mean=0
  Denominator=0
  for i in range(0,N):
    Mean=Mean+(X[i]*Weight[i])
    Denominator=Denominator+Weight[i]
    i=i+1
  return(str(round((Mean/Denominator),2)))
weighted_mean(5,[10, 40, 30, 50, 20],[1, 2, 3, 4, 5])
```
```python
example=list("abc")
int(input())
numbers = list(map(int, input().split(" ")))
weight = list(map(int, input().split(" ")))

print("%.1f" % (sum(list(map(lambda x : x[0] * x[1], zip(numbers, weight)))) / sum(weight)))
```
