#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

```python
a)  a = 0
    while (a < n * n * n):  #while a less than n^3 O(n^3)
      a = a + n * n   #a will become=  a + n*n
                    # a+ n*n < n*n*n
                    # divide n*n/n*n
                    #a < n
                    #becomes linear
                   # runtime: O(n)
```


```python
b)  sum = 0
    for i in range(n): #code enclosed will run for range n O(n)
      j = 1 #O(1) j=1 in this for loop 
      while j < n:  #code enclosed will run for range j< n O(n)
        j *= 2 #O(1) j grows 2 times in this while loop 
        sum += 1 #O(1)

        #O(n) * O(n)= runtime= O(n^2)
```

```python 
c)  def bunnyEars(bunnies): 
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1) #recursive call occurs once O(n), increases at linear rate with size of input 
      #runtime = O(n )
```

## Exercise II

-sort n list 
-Find min and max of  n-story building, determine that as range of n -story building
-find mid point of range (min + (max-low) /2)
-compare the value at mid point to check if its where f is (or where egg is broken), 
-comparison check: if the value at mid point, breaks egg, & the value to right of it (f+1), breaks egg, & value to left (f-1) does not break egg, return midpoint value as f, 
- if not keep searching: 
- if f-1 breaks egg, we know we are level(s) too high, so move midpoint -1, & repeat comparison heck, 
-else if midpoint does not break egg, but midpoint+1 break eggs, we know we need to move to right (midpoint +1) , and repeat comparison check

binary search!


O(log n)

