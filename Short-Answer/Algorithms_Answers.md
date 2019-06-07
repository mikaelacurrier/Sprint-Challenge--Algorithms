Add your answers to the Algorithms exercises here.

a) O(n)

b) O(n^4)

c) O(n)

Since we know how tall the building is, we can safely assume that _n_ >= _f_ > 0
The first solution would be a for loop that breaks when the egg is broken. This would be O(n)
A more time-effecient solution could be testing n/2. If the egg breaks, take that number and again divide by 2 until the correct floor is found. If the egg doesn't break, take the current floor, divide by n, multiply by the current floor and change the current floor to current + this number (and only allow intergers).
For example, n=10, the egg doesn't break at floor 5, (5/10 \* 5) + 5 = 7.5 so the current floor would be 7 and the test would run again.
This would be O(log(n))
