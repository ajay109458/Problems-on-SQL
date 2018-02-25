# Problem 4 - Occupatin

[Problem 4 - Occupation](https://www.hackerrank.com/contests/simply-sql/challenges/the-pads/problem)

## Solution 
SELECT CONCAT(NAME, CONCAT(CONCAT('(', LEFT(OCCUPATION,1 ))), ')')
FROM OCCUPATIONS
ORDER BY name;
SELECT CONCAT('There are a total of ', COUNT(OCCUPATION), ' ', LOWER(OCCUPATION), 's.') as a
FROM OCCUPATIONS
GROUP BY OCCUPATION
ORDER BY a, OCCUPATION
