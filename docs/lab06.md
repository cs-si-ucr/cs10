Exercise 1
---

Write a program that prints one random number in `[1, 6]`.


Exercise 2
---

Output a sideways "skyline" with random building heights.
Do not print an empty line as part of the skyline.
The maximum height building need not be part of the skyline, but no building should be taller.

Example:

> How many buildings? <u>**7**</u><br>
> How tall is the tallest building? <u>**9**</u><br>
> <br>
> XXXXXXX<br>
> XXX<br>
> XXXX<br>
> X<br>
> XXXXXXXXX<br>
> XXXX<br>
> XXXX


Exercise 3
---

Write a program that prints `n` random numbers in `[a, b]`.
The values for `n`, `a`, and `b` will come from the user.
`a` will be less than or equal to `b`.

Example:

> How many random numbers would you like? <u>**4**</u><br>
> What range should the numbers be in (space-separated)? <u>**-3 3**</u><br>
> Your random numbers are:<br>
> -2<br>
> 3<br>
> 1<br>
> -1

**Bonus**:
Allow the user to enter the numbers in the wrong order.
For instance, they could enter `3 -3` and your program would output numbers in `[-3, 3]`.


Exercise 4
---

Implement your own pseudo-random number generator.

HINT:
Be careful about big numbers.
Choose your datatypes accordingly.

Algorithm:

> Pick a number to mod by.
> We will be using **6947**.<br>
> Pick a number to shift by.
> We will be using **27**.<br>
> Pick a number to exponentiate by.
> We will be using **3**.<br>
> Start with some intial sequence value, called the *seed* (mod 6947)<br>
> The next term in the sequencee is the previous term plus the shift value, raised to the third power (mod 6947)

Example:

> Enter the seed value: <u>**0**</u><br>
> How many random numbers would you like? <u>**5**</u><br>
> 5789<br>
> 2500<br>
> 2438<br>
> 2844<br>
> 267


**Bonus**:

Use the current time to seed our random number generator.

