# Asymptotic-notation C++
Just a little script I put together to test a theory about asymptotic notation.
We want to know scalability of algorithm, how it behaves when input size grows (because data amount tend to increase).
That means the time required to any algorithm is depends on the number of inputs,
only for such algorithms we can calculate the time complexity by using Asymptotic notation.

YvoneBonam - Programmer at http://applianceauthority.org/air-fryers/air-fryers-shopping-guide-for-2015/

=============================================================
Simple complexity checking algo :

function find-min-plus-max(array a[1..n])
  // First, find the smallest element in the array
  let j := \infty;
  for i := 1 to n:
    j := min(j, a[i])
  repeat
  let minim := j
  
  // Now, find the biggest element, add it to the smallest and
  j := -\infty;
  for i := 1 to n:
    j := max(j, a[i])
  repeat
  let maxim := j
  
  // return the sum of the two
  return minim + maxim;
end

