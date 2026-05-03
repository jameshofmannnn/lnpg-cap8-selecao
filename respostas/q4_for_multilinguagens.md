a) Python

i = 0
j = 17
n = 100
sum = 0

while i < n:
    sum += i * j + 3
    i += 1
    j -= 1


b) JavaScript

let n = 100;
let sum = 0;

for (let i = 0, j = 17; i < n; i++, j--) {
    sum += i * j + 3;
}


c) C

int i, j, n = 100;
int sum = 0;

for (i = 0, j = 17; i < n; i++, j--) {
    sum += i * j + 3;
}


d) Ruby

i = 0
j = 17
n = 100
sum = 0

while i < n
  sum += i * j + 3
  i += 1
  j -= 1
end


e) SQL

WITH RECURSIVE loop(i, j, sum) AS (
  SELECT 0, 17, 0
  UNION ALL
  SELECT i + 1, j - 1, sum + (i * j + 3)
  FROM loop
  WHERE i < 99
)
SELECT sum FROM loop
ORDER BY i DESC
LIMIT 1;