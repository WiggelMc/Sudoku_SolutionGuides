<link rel="stylesheet" href="styles.css">
<div class="page-br"></div>

# Crudely Drawn Stickman
by Wiggel

## Solution Guide

### Initial Deductions

There are 15 possible sets of 4 digits from 1-6.
```
Number of Sets
= 6 choose 4
= 15
```

There are 15 groups in the puzzle that need unique sets, meaning all possible sets are used.
```
Total Groups
= 4 Rows + 4 Columns + 2 Diagonals + 5 Black Lines
= 15
```

<div class="page-br"></div>

Each Digit must appear in exactly 10 groups.
```
Groups, that digit X appears in
= 15 - Groups, that digit X doesn't appear in
= 15 - (5 choose 4)
= 15 - 5
= 10
```

Here are all cells, with the number of groups they are a part of.

<img src="assets/group_counts.png" width="256"/>

All Cells on the grid are either part of 3, 4, or 6 groups, that narrows down the possible ways for them to sum to 10. There are only 2 possibilities.
```
[3, 3, 4]
[4, 6]
```

<div class="page-br"></div>

### The Breakin

The two red cells each are part of 6 groups. <br>
We can conclude that they must pair up with a cell, thats part of 4 groups.<br>
These cells also see most of the grid, on account of being part of 6 groups.

Let us place a digit 'A' into one of those two red cells.<br>
It already sees all but 2 other cells in the grid.<br>
To add up to 10, we need to place the other 'A' into a purple cell.

<img src="assets/step_a1.png" width="256"/>
<img src="assets/step_a2.png" width="256"/>
<br><br>

The same can be done with the other red cell.<br>
We place a digit 'B', and we need another B in a purple cell.

<img src="assets/step_b1.png" width="256"/>
<img src="assets/step_b2.png" width="256"/>
<br><br>

Now we have placed all instances of the digits 'A' and 'B'.
Because those are the only digits in red cells, all other digits must each appear a total of 3 times in the grid.

```
[3, 3, 4] eg. [green, green, purple]
```

<div class="page-br"></div>

### Scaling down the domain

While it's possible to solve the puzzle, by just looking at 4 cell groups, it will still require at least some more complex steps.<br>
To scale the amount of groups down, we are looking only at groups containing both 'A' and 'B'.
```
Composition: [A B ? ?]
```

There are 6 such groups.
```
Number of Groups
= 4 choose 2
= 6
```

Each digit must appear in exactly 3 of those groups.
```
Groups, that digit X appears in
= 6 - Groups, that digit X doesn't appear in
= 6 - (3 choose 2)
= 6 - 3
= 3
```

Here are all cells, with the number of groups they are a part of.

<img src="assets/group_counts_ab.png" width="256"/>

All Cells on the grid are either part of 0, 1, or 2 groups, that narrows down the possible ways for them to sum to 3.<br>
Because we know that each digit appears 3 times in the grid, there are only 2 possibilities.
```
[1, 1, 1]
[0, 1, 2]
```

Let use place a digit 'C' into one of those two purple cells.<br>
We now need to place one 'C' each into a white and a green cell.<br>
We cannot place 'C' into the top white cell, because then both placed 'C's would be part of 4 groups globally.<br>
We know that the global composition is [3, 3, 4], so that doesn't work.<br>
So we place 'C' into the bottom  white cell, which narrows down the 'C' in green.

<img src="assets/step_c1.png" width="256"/>
<img src="assets/step_c2.png" width="256"/>
<br><br>

TODO

<img src="assets/step_d1.png" width="256"/>
<img src="assets/step_d2.png" width="256"/>
<img src="assets/step_d3.png" width="256"/>
<img src="assets/step_d4.png" width="256"/>
<br><br>

TODO

<div class="page-br"></div>

### E and F

TODO

<img src="assets/positions_ef.png" width="256"/>

TODO

<img src="assets/step_ef1.png" width="256"/>
<img src="assets/step_ef2.png" width="256"/>
<img src="assets/step_ef3.png" width="256"/>
<br><br>

TODO

<img src="assets/step_r1.png" width="256"/>
<img src="assets/step_r2.png" width="256"/>
<img src="assets/step_r3.png" width="256"/>
<br><br>

TODO

<div class="page-br"></div>

### Assigning Digits

TODO

<img src="assets/step_rn1.png" width="256"/>
<br><br>

TODO

<img src="assets/step_rn2.png" width="256"/>
<br><br>

TODO

<img src="assets/step_rn3.png" width="256"/>
<img src="assets/step_rn4.png" width="256"/>
<br><br>

TODO

<img src="assets/step_rn5.png" width="256"/>
<img src="assets/step_rn6.png" width="256"/>
<br><br>

TODO

