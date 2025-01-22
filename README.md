# Off-by-One Error in Java

This repository demonstrates a common off-by-one error in Java when iterating over arrays.  The provided code attempts to access an array element beyond its valid index, resulting in an `ArrayIndexOutOfBoundsException`.  A corrected version is also included to illustrate the proper way to handle array iteration.

**Bug:** The `for` loop in `bug.java` incorrectly uses `i <= arr.length` as the termination condition.  Arrays are zero-indexed, meaning valid indices range from 0 to `arr.length - 1`. Therefore, accessing `arr[arr.length]` will throw an exception.

**Solution:** The `bugSolution.java` file provides the corrected code, using the condition `i < arr.length` to prevent the error.