Exercise 1
---

Create a program that outputs a menu that asks the user to pick an option between 1 - 5. If the option is 5 then the program should exit. Options 1 - 4 will be for the rest of the exercises. If the output is not in the range from 1 - 5 then the program should alert the user that the option is invalid and ask the user to enter another option.

Until you implement the other exercises simply do nothing if the user chooses 1 - 4.

Example output:

> Lab 05 Menu<br>
> 1. Exercise 2<br>
> 2. Exercise 3<br>
> 3. Exercise 4<br>
> 4. Exercise 5<br>
> 5. Exit<br>

> Enter your choice: **1**

> Exercise 2 running<br>
> ...

> Lab 05 Menu<br>
> 1. Exercise 2<br>
> 2. Exercise 3<br>
> 3. Exercise 4<br>
> 4. Exercise 5<br>
> 5. Exit<br>

> Enter your choice: **6**

> Invalid choice, try again.<br>
> Enter your choice: **5**

> Goodbye!

Exercise 2
---

Modify your program from Exercise 1 to do the following when the user chooses option 1:

Ask the user to enter an integer *n* and print out a diamond whose center width is equal to (2 \* *n*) - 1.

Example output:

> Please enter an integer: **3**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;\*<br>
> &nbsp;&nbsp;\*\*\*<br>
> \*\*\*\*\*<br>
> &nbsp;&nbsp;\*\*\*<br>
> &nbsp;&nbsp;&nbsp;&nbsp;\*<br>


Exercise 3
---

Modify your program from Exercise 1 to do the following when the user chooses option 2:

Ask the user for a number and output the multiplication table up to and including that number.

Example output:

> Please enter a number: **4**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;&nbsp;4<br>
> 1&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;&nbsp;4<br>
> 2&nbsp;&nbsp;2&nbsp;&nbsp;4&nbsp;&nbsp;6&nbsp;&nbsp;8<br>
> 3&nbsp;&nbsp;3&nbsp;&nbsp;6&nbsp;&nbsp;9&nbsp;&nbsp;12<br>
> 4&nbsp;&nbsp;4&nbsp;&nbsp;8&nbsp;&nbsp;12&nbsp;&nbsp;16<br>

**Bonus**

Notice in the table above that the table become more skewed as the numbers get larger. Fix the problem by making the numbers right justified instead of left justified.

Example output for **Bonus**:
> Please enter a number: **4**<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4<br>
> 1&nbsp;&nbsp;1&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4<br>
> 2&nbsp;&nbsp;2&nbsp;&nbsp;4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8<br>
> 3&nbsp;&nbsp;3&nbsp;&nbsp;6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9&nbsp;&nbsp;12<br>
> 4&nbsp;&nbsp;4&nbsp;&nbsp;8&nbsp;&nbsp;12&nbsp;&nbsp;16<br>

Exercise 4
---

Modify your program from Exercise 1 to do the following when the user chooses option 3:

Ask the user for an integer and output the factorial of that integer. Don't use multiplication.

In case you're unfamiliar with what the factorial function does, here is a brief definition:<br>
1. The factorial of a number *n*, denoted *n*!, is given by *n*! == *n* \* (*n* - 1) \* (*n* - 2) \* ... \* 3 \* 2 \* 1.<br>
2. 0! == 1.<br>

Example output:

> Please enter an integer: **5**<br>
> 120

**Bonus**

If the user enters a negative or floating point number alert the user that their input is invalid and re-prompt the user.

Example output for **Bonus**:

> Please enter an integer: **-1**<br>
> Error: Invalid Input!<br>
> Please enter an integer: **0**<br>
> 1

Exercise 5
---

Modify your program from Exercise 1 to do the following when the user chooses option 4:

Ask the user to enter a word that is exactly 3 characters long and output all permutations of that word, 2 words on each line.

Example output:

> Enter a 3 letter word: **bug**<br>
> bug bgu<br> 
> ugb ubg<br>
> gub gbu 

Note that the order doesn't have to be exactly the same as above as long as all permutations are there.

**Bonus**

Modify Exercise 5 to allow a string of 4 characters and output all permutations of that word with 4 words on each line.

Quiz!
---
[quiz05](https://goo.gl/forms/NWbZ5G4ZiYieqh2B3)


