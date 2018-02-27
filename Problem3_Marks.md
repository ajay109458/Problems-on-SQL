## Problem

[Marks](https://www.hackerrank.com/contests/simply-sql/challenges/more-than-75-marks)

## Solution 
```
SELECT Name 
FROM STUDENTS
WHERE MARKS > 75
ORDER BY RIGHT(Name, 3), id
```
