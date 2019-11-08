#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This runs in O(n). Initially it looked like it would run in O(n^3), but then I 
realized it increments a by n^2 every time the loop runs. For example, if n=2, a 
starts as 0, the loop runs once and increments a to 2^2(4), then runs a second 
time and increments a to 8. So for n=2 the loop runs twice.



b) This run in O(n^2). There are nested loops, and even though the coefficient of
the inner loop may be small, that doesn't matter because coefficients are dropped
when figuring out time complexity.


c) bunnyEars is called recursively n times before reaching its base case. It's in 
linear time, O(n).

## Exercise II


