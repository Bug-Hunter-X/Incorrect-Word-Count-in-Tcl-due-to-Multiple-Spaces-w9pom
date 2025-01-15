# Tcl Word Count Bug

This repository demonstrates a common error in Tcl when counting words: the `split` command's behavior with multiple spaces.  The `bug.tcl` file contains code that incorrectly counts words due to this issue. The `bugSolution.tcl` file provides a corrected version.

## Bug Description
The `split` command in Tcl, by default, splits a string based on whitespace. If multiple spaces are present between words, the result is an incorrect word count. The provided example showcases this issue. 

## Solution
The solution involves using the `regexp` command to split the string based on one or more whitespace characters, ensuring accurate word counts regardless of spacing.