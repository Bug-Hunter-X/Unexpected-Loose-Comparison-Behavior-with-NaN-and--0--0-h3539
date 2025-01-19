# JavaScript Loose Comparison Bug: NaN and +/- 0

This repository demonstrates a common, yet easily overlooked, issue in JavaScript's loose comparison (==) operator. Specifically, the way it handles NaN (Not a Number) and positive/negative zero (+0, -0). 

**The Problem:**

*   `NaN == NaN` evaluates to `false`.  This is counterintuitive, as one would expect a value to be equal to itself.
*   `+0 == -0` evaluates to `true`. While mathematically these are distinct, JavaScript's loose comparison treats them as equivalent.

This can lead to incorrect program logic if not carefully considered.  The provided code demonstrates these unexpected behaviors. The solution file offers a corrected approach using strict equality (===).