# Incorrect Object Comparison in React's useEffect Hook
This example demonstrates a common error in React's `useEffect` hook when dealing with object comparisons.  The provided code attempts to compare two objects directly using the strict inequality operator (`!==`), which will not function as intended when comparing object references.  Object references are distinct, even if the objects have identical data; therefore the comparison will always return `true` except for the same object. This leads to unnecessary re-renders and potential performance issues.

The solution shows how to correctly compare objects by using a deep comparison library or manually checking properties.
