# Expose - Javascript Part 1

1. 'values added:  20'
2. 'final result:  20'
3. 'values added:  20'
4. ReferenceError: result is not defined.  Result is only accessible inside the if block, resulting in an error when accessed outside.
5. TypeError: Assignment to constant variable.  Setting the const result to 0 prohibits further re-assignments.
6. TypeError: Assignment to constant variable.  If result were not re-assigned it would then be a ReferenceError: result is not defined since it's only accessible in the if block.