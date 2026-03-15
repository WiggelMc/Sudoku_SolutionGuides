<link rel="stylesheet" href="styles.css">
<div class="page-br"></div>

# The Neighbour’s Rooftop Window

by Wiggel

## Solution Guide

<a href="https://sudokupad.app/leugsgup5u?setting-nogrid=1">Solve on SudokuPad</a>

<img src="assets/puzzle.png" width="512" />
<br><br>

<div class="page-br"></div>

### Rules

- Place the digits 1 to 9 once each in every row and column of the grid and once each into the circles of the cube.

- Reserved Neighbours: Digits in the grid may only be orthogonally adjacent, if they share an edge on the cube.
  (Eg. If R1C1 contained a 1, and R1C2 a 2, then 1 and 2 would need to be connected on the cube, for example in R10C13 and R11C14.)

- Arrows: Digits along an arrow sum to the number in the attached circle. Cells outside the grid are empty and do not count towards that sum.

- Killer Cages: Digits cannot repeat within a cage.

<br><br>

<div class="page-br"></div>

### Spoiler Warning

<br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

<div class="page-br"></div>

### Initial Deductions

- The digit in the middle of the cube can only have two distinct neighbours.
- We construct an example layout, that may be rotated or mirrored.

<img src="assets/a1.png" width="512"/>
<br><br><div class="page-br"></div>

- Only 'A' can be adjacent to both 'B' and 'C', so the placement of those dictates, where 'A' must go.

<img src="assets/a2.png" width="512"/>
<br><br><div class="page-br"></div>

- We can extend this logic towards the edge of the grid.

<img src="assets/a3.png" width="512"/>
<br><br><div class="page-br"></div>

- The highest 'B' or 'C' places the 'A' on the other edge, because only one neighbour of 'A' is left in that row.
- So the final grid must have a wrapping diagonal of 'A', with 'B' on one side and 'C' on the other.

<img src="assets/a4.png" width="512"/>
<br><br><div class="page-br"></div>

### The Diagonal

- 'A' cannot be placed inside the cage, because it would force 'A' to repeat in the cage.

<img src="assets/b1.png" width="512"/>
<br><br><div class="page-br"></div>

- The digits in the cage must correspond to a side of the cube to satisfy the geometry without repeats.
- Any side contains either 'B' or 'C', so one of them must be present in the cage.

<img src="assets/b2.png" width="512"/>
<br><br><div class="page-br"></div>

- The presence of 'B' or 'C' in the cage forces one of 4 possible positions for the diagonal.

<img src="assets/b3.png" width="512"/>
<br><br><div class="page-br"></div>

- The orange diagonal would force another 'BC' on the cube, but we have both placed already.

<img src="assets/b4.png" width="512"/>
<br><br><div class="page-br"></div>

- The same logic can be used to rule out the gray diagonal.

<img src="assets/b5.png" width="512"/>
<br><br><div class="page-br"></div>

- To rule out the green diagonal, we set 'B' and 'C' on the cube.
- The digit on the 'B' arrow must be 'C', because 'A' cannot be 0. 

<img src="assets/b6.png" width="512"/>
<br><br><div class="page-br"></div>

- If we now declare the digit on the small arrow as 'D', we can measure their distance to 'B' without going through 'A'.
- Because the cube without 'A' can be colored in two colors in a checkerboard arrangement, all paths between two digits not going through 'A' will have the same parity.
- In the grid, the distance between 'B' and 'D' is 4, eg. it's even. On the cube the distance is 1, eg. it's odd.
- The parities don't match, therefore it is impossible to have a valid path between them in the grid.

<img src="assets/b7.png" width="512"/>
<br><br><div class="page-br"></div>

- We can now place the purple diagonal.

<img src="assets/b8.png" width="512"/>
<br><br><div class="page-br"></div>

- Because the parity does not match, the upper 'BC' on the cube cannot be 'C'.

<img src="assets/b9.png" width="512"/>
<br><br><div class="page-br"></div>

- We can resolve 'B' and 'C' on the cube.
- All digits from 'A', 'B' and 'C' have now been placed.

<img src="assets/b10.png" width="512"/>
<br><br><div class="page-br"></div>

### Grid Geometry

- We can now color the remaining digits on the cube based on their parity.

<img src="assets/c1.png" width="512"/>
<br><br><div class="page-br"></div>

- This coloring can be translated into the grid based, because purple must be next to 'C' and green must be next to 'B'.

<img src="assets/c2.png" width="512"/>
<br><br><div class="page-br"></div>

- We can now label the other digits and slowly resolve them using sudoku.
- Two different digits of the same color like 'EF' will always have only one option from the other color available, like 'G'.
- We label new digits on the cube, whenever we need them.
- Sometimes we have two options for labeling, where both are equally valid. In that case, we pick one, because they will lead to the same solution. Of course this only applies, if we have not placed any of those labels before. For example, we have both 'HI' pairs on the cube and in the grid without having placed 'H' or 'I' anywhere. There is no distinction between 'H' and 'I', so we can select one of them to set as 'H'.

<p>
<img src="assets/c3.png" width="400"/>
<img src="assets/c4.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/c5.png" width="400"/>
<img src="assets/c6.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/c7.png" width="400"/>
<img src="assets/c8.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/c9.png" width="400"/>
<img src="assets/c10.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d1.png" width="400"/>
<img src="assets/d2.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d3.png" width="400"/>
<img src="assets/d4.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d5.png" width="400"/>
<img src="assets/d6.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d7.png" width="400"/>
<img src="assets/d8.png" width="400"/>
</p>
<br><br><div class="page-br"></div>

- We set 'E' to be the digit next to 'H'.
- Therefore 'F' will be next to 'I'.

<p>
<img src="assets/d9.png" width="400"/>
<img src="assets/d10.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d11.png" width="400"/>
<img src="assets/d12.png" width="400"/>
</p>
<br><br>
<p>
<img src="assets/d13.png" width="400"/>
<img src="assets/d14.png" width="400"/>
</p>
<br><br><div class="page-br"></div>

### Assigning Digits

- After resolving the digits in the grid, the 'HI' and 'EF' pairs on the cube remain unresolved.
- For resolving them, we can look cat the two leftmost arrows.
- The left arrow requires 'I' to be less than 'C'.
- The second arrow therefore cannot sum to 'I', because then 'C' would also have to be less than 'I'.

<img src="assets/e1.png" width="512"/>
<br><br><div class="page-br"></div>

- We can resolve 'H' and 'I'.
- Because we know that 'E' is next to 'H', we can resolve 'E' and 'F' as well.

<img src="assets/e2.png" width="512"/>
<br><br><div class="page-br"></div>

- Now we have all digits labeled.

<img src="assets/e3.png" width="512"/>
<br><br><div class="page-br"></div>

- We can write down the four outer arrows as equations.

```
C = A + E + I
H = A + C
B = E + G
F = B + 2I

TODO
```

<img src="assets/e4.png" width="512"/>
<br><br><div class="page-br"></div>
