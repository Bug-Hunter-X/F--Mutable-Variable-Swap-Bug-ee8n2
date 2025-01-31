# F# Mutable Variable Swap Bug

This repository demonstrates a common error in F# when working with mutable variables and attempting to swap their values. The issue arises from a misunderstanding of how variables are handled in F#. In F#, variables are passed by value, not by reference. This means that the `swap` function receives copies of the variables, and any modifications within the function do not affect the original variables.

## Bug

The original `bug.fs` file contains a function `swap` which attempts to swap two mutable variables, `x` and `y`. However, the swap does not work correctly because of how F# passes function parameters.