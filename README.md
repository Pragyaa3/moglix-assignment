## moglix-assignment
# Longest Valid Parentheses

Moglix online shortlisting assignment.

## Problem
Given a string of only `(` and `)`, find the length of the longest valid (well-formed) parentheses substring.

Example: `")()())"` → `4` (because `"()()"` is valid)

## Approach
Used a stack to store indices.
- Push index of every `(`
- On `)`, pop the top. If stack is empty, push current index as new base. Otherwise, current valid length = `i - stack.peek()`

O(n) time, O(n) space.

## Run it
```bash
javac LongestValidParentheses.java
java LongestValidParentheses
```