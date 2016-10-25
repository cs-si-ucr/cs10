Exercise 1
---

Write a program that outputs a menu that asks the user to pick an option between 1 - 6.
If the option is 6 then the program should exit.
Options 1 - 5 will be for the exercises.
If the output is not in the range from 1 - 6 then the program should alert the user that the option is invalid and ask the user to enter another option.

Until you implement the other exercises simply do nothing if the user chooses 2 - 5.
All of the exercises for this week will go in this file.

Example output:

> Lab 05 Menu<br>
> 1. Do nothing<br>
> 2. Exercise 2<br>
> 3. Exercise 3<br>
> 4. Exercise 4<br>
> 5. Exercise 5<br>
> 6. Exit
>
> Enter your choice: **1**
>
> Lab 05 Menu<br>
> 1. Do nothing<br>
> 2. Exercise 2<br>
> 3. Exercise 3<br>
> 4. Exercise 4<br>
> 5. Exercise 5<br>
> 6. Exit
>
> Enter your choice: **7**<br>
> Invalid choice, try again.<br>
> Enter your choice: **6**
>
> Goodbye!

Another example:

> Lab 05 Menu<br>
> 1. Do nothing<br>
> 2. Exercise 2<br>
> 3. Exercise 3<br>
> 4. Exercise 4<br>
> 5. Exercise 5<br>
> 6. Exit
>
> Enter your choice: **2**
>
> Executing exercise 2...<br>
> (exercise 2 runs here)
>
> Lab 05 Menu<br>
> 1. Do nothing<br>
> 2. Exercise 2<br>
> 3. Exercise 3<br>
> 4. Exercise 4<br>
> 5. Exercise 5<br>
> 6. Exit
>
> Enter your choice: **6**
>
> Goodbye!


Exercise 2
---

Ask the user to enter a word that is exactly 3 characters long and output all permutations of that word.
Output 1 permutation of the word per line.

Example output:

> Enter a 3 letter word: **bug**<br>
> bbb<br>
> bbu<br>
> bbg<br>
> bub<br>
> buu<br>
> bug<br>
> bgb<br>
> bgu<br>
> bgg<br>
> ubb<br>
> ubu<br>
> ubg<br>
> uub<br>
> uuu<br>
> uug<br>
> ugb<br>
> ugu<br>
> ugg<br>
> gbb<br>
> gbu<br>
> gbg<br>
> gub<br>
> guu<br>
> gug<br>
> ggb<br>
> ggu<br>
> ggg

Note that the order does not have to be exactly the same as above as long as all permutations are there (this order is the easiest, though).

**Bonus**

Allow a string of 4 characters and output all permutations of that word with 4 words on each line.


Exercise 3
---

Ask the user for a number and output the multiplication table up to and including that number.

Example output:

> Please enter a number: **4**<br>
> 1&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;&nbsp;4<br>
> 2&nbsp;&nbsp;4&nbsp;&nbsp;6&nbsp;&nbsp;8<br>
> 3&nbsp;&nbsp;6&nbsp;&nbsp;9&nbsp;&nbsp;12<br>
> 4&nbsp;&nbsp;8&nbsp;&nbsp;12&nbsp;&nbsp;16<br>

**Bonus 1**

Add row and column numbers to your output

Example output for **Bonus 1**:

> Please enter a number: **4**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;&nbsp;4<br>
> 1&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;&nbsp;4<br>
> 2&nbsp;&nbsp;2&nbsp;&nbsp;4&nbsp;&nbsp;6&nbsp;&nbsp;8<br>
> 3&nbsp;&nbsp;3&nbsp;&nbsp;6&nbsp;&nbsp;9&nbsp;&nbsp;12<br>
> 4&nbsp;&nbsp;4&nbsp;&nbsp;8&nbsp;&nbsp;12&nbsp;&nbsp;16<br>

**Bonus 2**

Notice in the table above that the table become more skewed as the numbers get larger.
Fix the problem by making the numbers right justified instead of left justified.

Example output for **Bonus 2**:

> Please enter a number: **4**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4<br>
> 1&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4<br>
> 2&nbsp;&nbsp;2&nbsp;&nbsp;4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8<br>
> 3&nbsp;&nbsp;3&nbsp;&nbsp;6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9&nbsp;&nbsp;12<br>
> 4&nbsp;&nbsp;4&nbsp;&nbsp;8&nbsp;&nbsp;12&nbsp;&nbsp;16<br>


Exercise 4
---

Ask the user to enter an integer ``n`` and print out a diamond whose center width is equal to ``(2 * n) - 1``.

Example output:

> Please enter an integer: **3**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;\*<br>
> &nbsp;&nbsp;\*\*\*<br>
> \*\*\*\*\*<br>
> &nbsp;&nbsp;\*\*\*<br>
> &nbsp;&nbsp;&nbsp;&nbsp;\*<br>


Exercise 5
---

Ask the user for an integer and output the factorial of that integer. Do not use multiplication.

In case you are unfamiliar with what the factorial function does, here is a brief definition:

>1. The factorial of a number ``n``, denoted ``n!``, is given by ``n! == n * (n-1) * (n-2) * (n-3) * ... * 3 * 2 * 1``<br>
>2. The special case of ``n == 0`` is defined as follows:<br>
>3. ``0! == 1``

Example output:

> Please enter an integer: **5**<br>
> 5! == 120

**Bonus**

If the user enters a negative or floating point number alert the user that their input is invalid and re-prompt the user.

Example output 1 for **Bonus**:

> Please enter an integer: **-1**<br>
> Error: Invalid Input!<br>
> Please enter an integer: **0**<br>
> 1

Example output 2 for **Bonus**:

> Please enter an integer: **1.4**<br>
> Error: Invalid Input!<br>
> Please enter an integer: **3.0**<br>
> 6



Quiz!
---
[quiz05](https://goo.gl/forms/NWbZ5G4ZiYieqh2B3)


