## Problem

[The Report](https://www.hackerrank.com/contests/simply-sql/challenges/the-report)

## Solution
```
SELECT if(g.grade < 8, NULL, s.name) as n, g.grade, s.marks
FROM STUDENTS s
JOIN GRADES g
  ON  s.MARKS >= g.MIN_MARK  
  AND s.MARKS <= g.MAX_MARK
ORDER BY g.grade desc, s.name, s.marks
```
