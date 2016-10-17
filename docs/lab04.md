Exercise 1
---

Take in a string from the user and print it back out repeatedly with each print having one less
character on the end. Stop printing once there are no more chars in the string left to print.

Example:

> Enter a string: **Test**</br>
> Test </br>
> Tes </br>
> Te </br>
> T

Exercise 2
---

Take in two integers from the user and multiply them without using the multiplication operator ``*``
Then, output the result.

Example:

> Enter two numbers: **5 6** </br>
> 5 * 6 = 30

Exercise 3
---

Create a program that implements the collatz conjecture. The collatz conjecture can be summarized 
as follows:<br>
Take any positive integer n. If n is even, divide it by two. If n is odd, multiply it by 3 and add
one. Repeat this process for the new n. Eventually, no matter what number n is, it will end up as 1.<br>
Create this program by taking in an integer from the user and then performing the collatz 
conjecture algorithm on it. Print out the number each time it gets changed to show the steps it 
took that number to reach 1.

Example:

> Enter an integer: **5**</br>
> 5</br>
> 16</br>
> 8</br>
> 4</br>
> 2</br>
> 1

Hint:
Take a look at the collatz conjecture on wikipedia:
[click here](https://en.wikipedia.org/wiki/Collatz_conjecture)

Exercise 4
---

Create a program that takes in a user string and reverses it. (Bonus: if it is a palindrome, output a sentnce saying so).

Example 1:

> Enter a string: **Andre Castro**<br>
> ortsaC erdnA

Example 2:

> Enter a string: **lionoil**<br>
> lionoil<br>
> lionoil is a palindrome!

Exercise 5
---

Create a password protected program where the user has to guess a password in a certain amount of
tries. The amount of times should be at least 4 but the max is up to you. Read a single string as
the password and output a hint eachtime the user gets it wrong (until you run out of hints).
(Bonus: treat words with lowercase and uppercase letters the same, ex: WorD and woRd should both
be considered correct by the program)

Example 1:

> Enter a word: **Test** <br>
> The word "Test" is incorrect. Hint: it is green.<br>
> Enter another word: **Grass**<br>
> The word "Grass" is correct!

Exmaple 2:

> Enter a word: **Temporary**<br>
> The word is incorrect. Hint: it starts with s<br>
> Enter another word: **Sentence**<br>
> The word is incorrect. Hint: it starts with s<br>
> Enter another word: **Stilts**<br>
> The word is incorrect. Hint: it starts with s<br>
> Enter another word: **Sit**<br>
> The word is incorrect. Hint: it starts with s<br>
> Enter another word: **Stow**<br>
> Im sorry. You failed to guesss the word. Goodbye.

Quiz!
---
[quiz03]()

