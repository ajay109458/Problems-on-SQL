## Problem

[EMPLOYEES](https://www.hackerrank.com/contests/simply-sql/challenges/the-blunder)

## Solution
```
SELECT CEIL(AVG(salary) - AVG(Replace(Salary, '0', '')))
FROM EMPLOYEES 
```
