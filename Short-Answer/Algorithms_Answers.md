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

First, I would call the first the lowest possible and the nth floor the highest 
possible. I would determine the middle floor between the lowest possible and the
highest possible.

Then, I would go to the middle floor and drop the egg.

If the egg broke, I'd label the middle floor as the highest possible and restart 
the process.

If the egg didn't break, I'd label the middle floor as the lowest possible and 
restart the process.

Before restarting the process, I'd check to see if lowest possible was one floor 
below highest possible. If it was, I'd stop and report that lowest possible was 
the highest floor you could toss an egg from without it breaking.

The runtime is O(log n) since this is essentially a binary search.