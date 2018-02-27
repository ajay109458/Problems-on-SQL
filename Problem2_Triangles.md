## Problem

[Triangles](https://www.hackerrank.com/contests/simply-sql/challenges/what-type-of-triangle)

## Solution
```
SELECT IF( A + B <= C OR B + C <= A OR C + A <= B , 
              "Not A Triangle",
              IF(A = B AND C = A, 
                   "Equilateral", 
                   IF(A = B OR B = C OR C = A, 
                       "Isosceles", 
                       "Scalene"))) 
FROM TRIANGLES
```
