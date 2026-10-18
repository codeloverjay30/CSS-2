# z-index
## intro
Many elements can overlap with `z-index` field. None of them dispear when they overlap.

## principle
To determine which one is on top layer when many items overlap, follow these rules.

+ The higher priority it has, the frontier it is placed.

To know the priority, follow these rules.

+ The value of `z-index` of the element is greater, the higher priority it has.

+ If there exist two same value of `z-index` in two or more different elements, 

then latter one one element is declared, the higher priority it has.
