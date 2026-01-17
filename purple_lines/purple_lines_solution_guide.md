<link rel="stylesheet" href="styles.css">
<div class="page-br"></div>

# Purple Lines

by Wiggel

## Solution Guide

<a href="https://sudokupad.app/56e3pocc01">Solve on SudokuPad</a>

<img src="assets/puzzle.png" width="512" />
<br><br>

<div class="page-br"></div>

### Rules

Normal sudoku rules apply: Place the digits 1 to 9 once each, in every row, column and box.

The grid is covered in fog, placing correct digits clears the fog somewhere in the grid.
No guessing is required, of course.

Blue lines are Modular Lines, every connected run of 3 cells along them must contain one digit each from each modular set
[147 258 369].

Red lines are Parity Lines, when going along them, digits alternate between odd and even.

Purple lines, ... - What? The title mentions purple lines?
What were they again? Maybe they were Renbans?
The digits on a Renban form a set of consecutive, non-repeating digits in any order.

No, that was wrong! No purple line could ever be a valid Renban.
Ah, now I remember! They just combine the rules of the other two lines.
So a purple line is always a valid blue line and a valid red line.
At the same time! Good thing I remembered that.

Now that I'm done explaining the rules, I have to get going.
I really hope the rules will help you with solving the puzzle.

<div class="page-br"></div>

### Spoiler Warning

If you have not played the puzzle before, I implore you to do so before you read this guide.<br>
The puzzle is not very hard and the solution guide does the process of solving it a disservice.<br>

You have been warned.
<br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

<div class="page-br"></div>

### Fog Clearing

- The ends of the blue line have to be from the same modular set.
- They cannot be from '147', because there is a '1' on the line.
- They also cannot be from '258', because 2 of those digits are already used.
- So they are from '369'.
- The other digit on the line then must be '8', the last digit from '258'.
  <br><br>
- The '4' can only be placed in the bottom left cell, because the free cells on the red line must be odd.

<img src="assets/s1.png" width="512"/>
<br><br><div class="page-br"></div>

- The revealed given '7' places a '7' in box 8 by sudoku.

<img src="assets/s2.png" width="512"/>
<br><br><div class="page-br"></div>

- The bottom two cells on the red line in box 9 must contain an odd digit.
- They both see the digits '3579', so they must contain a 1.
  <br><br>
- The blue line in box 7 must contain a digit from '147', but only 1 is available.
- By sudoku, '1' must be in the bottom cell.

<img src="assets/s3.png" width="512"/>
<br><br><div class="page-br"></div>

- The blue line in box 4 must contain a digit from '147', which can only go into the top cell.
- The bottom cell therefore must be from '258' and only '2' is available.

<img src="assets/s4.png" width="512"/>
<br><br><div class="page-br"></div>

- The revealed given '7' makes the top cell of the blue line a '4' by sudoku.

<img src="assets/s5.png" width="512"/>
<br><br><div class="page-br"></div>

- The '7's in boxes 4 and 5 place the '7' in box 6 in row 6.
- Two cells on the line have to be even by parity line, so the '7' has to be in the remaining cell.

<img src="assets/s6.png" width="512"/>
<br><br><div class="page-br"></div>

- The revealed given '1' makes the left cell of the red line a '1' by sudoku.
- The other two digits on the red line have to be even by parity line.
- The top cell sees the digits '248', therefore it is a '6'.

<img src="assets/s7.png" width="512"/>
<br><br><div class="page-br"></div>

- The digits in row 4 on the newly revealed blue line must contain one digit from '147'.
- '71' are ruled out by sudoku in the row.
- '4' is ruled out from two of the columns, so '4' can be placed in the rightmost cell.

<img src="assets/s8.png" width="512"/>
<br><br><div class="page-br"></div>

- By sudoku and parity line, '1' in box 5 has to be in column 5.
- The digits in box 2 on the newly revealed blue line must contain one digit from '147'.
- All of them are ruled out of the right cells by sudoku in the column.
- In the leftmost cell, '14' are ruled out by sudoku in the column, so '7' can be placed there.

<img src="assets/s9.png" width="512"/>
<br><br><div class="page-br"></div>

- By sudoku, '4' and '7' in box 1 must be in column 2.
- By modular line, they cannot go into the center cell.
- '1' in column 2 must be in box 4, but the blue line in box 4 must contain a digit from '147' with '47' ruled out. So '1' must be placed, where column 1 and the line intersect.
  <br><br>
- '1' can now be placed in box 5 by sudoku

<img src="assets/s10.png" width="512"/>
<br><br>

<div class="page-br"></div>

### The Twist

At this point, no more digits can be placed without noticing a change in the puzzle.<br>
All of the lines have gradually turned purple.<br>
This change can be noticed earlier, but only at this point is it required to progress.<br>

<div class="page-br"></div>

### Purple Lines

Now all cells can be colored odd/even, because they must alternate on each line.<br>
Taking into account, that each row, column and box contains 4 even and 5 odd digits, more cells can be colored.<br>
The interactions of parity and modular lines resolve most of the puzzle.<br>
There are many possible paths from this point forward.<br>

<img src="assets/t1.png" width="256"/>
<img src="assets/t2.png" width="256"/>
<br><br>
<img src="assets/t3.png" width="256"/>
<img src="assets/t5.png" width="256"/>
<br><br>
<img src="assets/t6.png" width="256"/>
<img src="assets/t7.png" width="256"/>
<br><br>

<div class="page-br"></div>

### The Deadly Pattern

After all of the modular and parity logic has been used, a deadly pattern remains in the grid.<br>
At this point, the deadly pattern prompts the solver to read the rules again.<br>
The rules mention that a purple line could never be a valid Renban. This resolves the deadly pattern, by looking in box 5.<br>
It can also be resolved earlier by those who have noticed the hidden rule in the text at an earlier point.<br>

<img src="assets/u1.png" width="512"/>
<br><br>
<img src="assets/u2.png" width="512"/>
<br><br>

<div class="page-br"></div>

### Stylistic Decisions

The reason, the rules are worded a lot more casually than usual, is to make the solver less sure about the rules.
The ending paragraph is especially useful, because it contains no information, similarly to how 'Foggy on the Details' by ThePedalingPianist and juggler did it.

I think this a necessary step to make a twist work properly. The solver needs to be in the correct headspace for that.

I needed some filler text to make sure the twist will not be guessed. That is why I talk about Renbans before actually explaining what purple lines do.
I did not want that diversion to be fully useless, that's why I added the non-Renban constraint, that is needed to disambiguate a deadly pattern.