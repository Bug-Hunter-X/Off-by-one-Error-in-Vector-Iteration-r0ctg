# Off-by-One Error in C++ Vector Iteration

This example demonstrates a common off-by-one error when iterating over a `std::vector` in C++.  The loop condition `i <= vec.size()` is incorrect.  Vectors are 0-indexed, so the last valid index is `vec.size() - 1`.

The `bug.cpp` file contains the erroneous code. The `bugSolution.cpp` file provides the corrected version.

## How to Reproduce

1. Compile `bug.cpp`.
2. Run the executable.  It will likely crash or produce undefined behavior due to accessing memory outside the vector's bounds.
3. Compile and run `bugSolution.cpp` to see the correct output.