#### The devide and conquer 
1. Devide into small problems
2. Conquer via recoursive calls

### Eg1: Find number of inversion pairs in an array:

1. **Brute Force**: O(n^2) time

set a double for-loop: i and j 

```
for i in xxx:
  for j=i+1 in xxx:
    if array[i]<array[j]:
      xxxxxxx
```
2. **Merge sort**
inversion pair (i,j)

* left version: if i,j< N/2

* right version: if i,j > N/2

* spilt version: if i < N/2 < j

a. devide array into two parts (X,Y)--> get number of inversions in X and Y--> x and y

b. sort X and Y separately

c. directly combine sorted X and sorted Y into Z--> get number of inversions in Z-->z

d. number of inversion pairs= x+y+y

### Eg2: Find cloest dots

**1D**:
1. sort dots(  O(n log n) )
2. find closet dots ( O(n) )

**2D:**
1. p_X/p_Y for points in x/y coordinate,
2. sort p_X/p_Y--> p_x/p_y  **O(n log n)**

