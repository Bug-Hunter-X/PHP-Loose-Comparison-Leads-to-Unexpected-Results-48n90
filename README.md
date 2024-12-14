# PHP Loose Comparison Bug

This repository demonstrates a common, yet often overlooked, issue in PHP: unexpected behavior arising from loose comparisons (==) when dealing with strings and integers. Specifically, the string '0' and the integer 0 are considered equal using loose comparison, while they are considered different using strict comparison (===). This can lead to subtle and hard-to-find bugs in your code.

## Bug Description
The `bug.php` file contains code that showcases this issue. The comparison using `==` returns `true`, while the comparison using `===` returns `false`, highlighting the difference between loose and strict comparison.

## Solution
The `bugSolution.php` file demonstrates how to correct the code by using strict comparison (===) to avoid unexpected results.  Strict comparison ensures that both the value and type of variables are checked before comparison.  This ensures the intended behaviour is achieved.