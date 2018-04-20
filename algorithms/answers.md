1.
  a. This would be a O(1) complexity, constant time, due to it coming down to a     = 2n no matter how big n becomes it is only one calculation.

  b. This would be O(n) complexity, linear time. It is looping and constantly       changing i to halve itself, increasing the time it takes to do so linearly     as n approaches infinity.

  c. Due to double nested for-loops, this would be O(n^3), cubic time. The          larger n becomes, sum quickly becomes very large, taking a long time to        calculate.

  d. Again due to a nested for-loop, this would be O(n^2), quadratic time. 

  e. This one also would be another exponential runtime as n gets larger, O(n^4)    specifically.

  f. This would be a linear time complexity recursive function. Run time            increases directly dependent on how big n is until it returns 0. 

  g. This is a recursive function searching each element in an array, therefore     it is of linear time complexity as well, because the first if statement is     only checking for a non-negative arraySize, each loop only checking one        item in constant time.

2.
  a. let a = [];
     a.length = n;
     let j = n - 1;
     let current = 0;
     for (let i = 0; i < n - 1; i++) {
       if (j > 0) {
         return Math.max(current, a[j--] - a[i]);
       }
     }
     return current;

  b. Start at floor n/2 and drop an egg, if it breaks then move to floor n/4 to     drop another, if it does not break then move to floor 3n/4. Continue this      method until f is determined. Splitting the floors in a binary search will     be most efficient to determine f. 

3.
  a. The first element being chosen as the pivot results in the worst-case run      time for quicksort, which would be quadratic time. This is because the         pivot splits quicksort into multiple sorts recursively. If it is fully         sorted then all elements will go into the greater array in each recursion,     causing the maximum number of calls to be made, nested length minus one        calls.

  b. Always picking the median element will result in the fewest recursive calls,   resulting in a best-case scenario for running time. In the case of             quicksort this would be O(n log n) or O(n), depending how it is                implemented. This is due to the most even split possible between the less      and greater sorts, resulting in fewer recursion and nesting.