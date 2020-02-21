#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n).
The loop is executed n times.


b) O(n log n).
The `for` loop runs n times, and the `while` loop runs log n times.


c) O(n).
The function recurses n times.

## Exercise II
def find_f(n):
  breaking_floor = n
  safe_floor = 0
  while True:
    this_floor = safe_floor + ((breaking_floor - safe_floor) // 2)
    if broken(this_floor):
      breaking_floor = this_floor      
    else:
      safe_floor = this_floor
      if breaking_floor == safe_floor + 1:
        return breaking_floor

This solution runs in time O(log n) using divide and conquer.
