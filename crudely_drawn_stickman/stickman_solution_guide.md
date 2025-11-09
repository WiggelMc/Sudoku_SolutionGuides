<link rel="stylesheet" href="styles.css">
<div class="page-br"></div>

# Crudely Drawn Stickman
by Wiggel

## Solution Guide

### Expected Deductions

There are 15 possible sets of 4 digits from 1-6.
```
Number of sets
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

### A and B

<img src="assets/step_a1.png" width="256"/>
<img src="assets/step_a2.png" width="256"/>
<img src="assets/step_b1.png" width="256"/>
<img src="assets/step_b2.png" width="256"/>

<div class="page-br"></div>

### C and D

<img src="assets/group_counts_ab.png" width="256"/>
<img src="assets/step_c1.png" width="256"/>
<img src="assets/step_c2.png" width="256"/>
<img src="assets/step_d1.png" width="256"/>
<img src="assets/step_d2.png" width="256"/>
<img src="assets/step_d3.png" width="256"/>
<img src="assets/step_d4.png" width="256"/>

<div class="page-br"></div>

### E and F

<img src="assets/positions_ef.png" width="256"/>
<img src="assets/step_ef1.png" width="256"/>
<img src="assets/step_ef2.png" width="256"/>
<img src="assets/step_ef3.png" width="256"/>
<img src="assets/step_r1.png" width="256"/>
<img src="assets/step_r2.png" width="256"/>
<img src="assets/step_r3.png" width="256"/>

<div class="page-br"></div>

### Assigning Digits

<img src="assets/step_rn1.png" width="256"/>
<img src="assets/step_rn2.png" width="256"/>
<img src="assets/step_rn3.png" width="256"/>
<img src="assets/step_rn4.png" width="256"/>
<img src="assets/step_rn5.png" width="256"/>
<img src="assets/step_rn6.png" width="256"/>

