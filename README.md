# Undefined Variable Bug in Haskell

This repository demonstrates a common runtime error in Haskell programs: using an undefined variable.

The `bug.hs` file contains the buggy code.  The `bugSolution.hs` file provides a corrected version.

## How to reproduce
1. Save `bug.hs`
2. Compile and run using a Haskell compiler (like GHC): `ghc bug.hs && ./bug`

You'll observe a runtime error indicating that the variable `x` is undefined.

## Solution
The solution involves providing a concrete value to the variable `x` or changing the logic such that `x` does not depend on an undefined value. This is often the result of improper function composition, or forgetting to define a variable's value within a local scope before usage.  Consider using pattern matching and case statements to handle various input scenarios explicitly.