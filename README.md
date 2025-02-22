# Haskell Maybe Type Error: fromJust Exception
This repository demonstrates a common error in Haskell when working with the Maybe type: using `fromJust` without first checking for the `Nothing` case.  The `fromJust` function is unsafe and will throw an exception if applied to `Nothing`. This example highlights the issue and provides a safe alternative. 

## Bug
The `bug.hs` file contains code that uses `fromJust` directly on a Maybe value that could potentially be `Nothing`. This results in an exception when executed.

## Solution
The `bugSolution.hs` file provides a corrected version that utilizes pattern matching or the `maybe` function to handle both the `Just` and `Nothing` cases gracefully, avoiding the exception.