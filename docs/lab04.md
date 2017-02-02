Exercise 1
---

Get a word from the user.
Repeat the word, removing one letter at a time (see example below).
Stop printing when there are no more characters.

**Bonus 1**:
Get an entire line of text from the user.

**Bonus 2**:
Always reduce the printed word by one *visible* character (spaces are not visible).
There is a function in the `cctype` library that you may use to determine if a character is a space or not.

Example:

> Enter a word: <u>**Test**</u></br>
> Test </br>
> Tes </br>
> Te </br>
> T

Bonus 2 Example:

> Enter a phrase: <u>**Hey there!**</u></br>
> Hey there</br>
> Hey ther</br>
> Hey the</br>
> Hey th</br>
> Hey t</br>
> Hey</br>
> He</br>
> H</br>

An **incorrect** version of bonus 2:

> Enter a phrase: <u>**Hey there!**</u></br>
> Hey there</br>
> Hey ther</br>
> Hey the</br>
> Hey th</br>
> Hey t</br>
> Hey</br>
> Hey</br>
> He</br>
> H</br>

(notice the repetition)


Exercise 2
---

Get two integers from the user and multiply them without using the `*` operator.

Example:

> Enter two numbers: <u>**5 6**</u></br>
> 5 * 6 = 30

**Bonus**:

Consider the input cases `10000 2` and `2 10000`.
Modify your code so you loop as few times as possible in both cases.


Exercise 3
---

Write a program that prints a collatz conjecture sequence.
The collatz conjecture is defined as follows:

> Take any positive integer ``n``<br>
> If ``n`` is even, divide it by two.<br>
> If ``n`` is odd, multiply it by 3 and add 1<br>
> Repeat this until ``n == 1``<br>

The collatz conjecture states that no matter what ``n`` you choose, you will always end up at 1.
No one has found a number that does not satisfy this conjecture.
No one knows why.

Example:

> Enter an integer: **3**</br>
> 10</br>
> 5</br>
> 16</br>
> 8</br>
> 4</br>
> 2</br>
> 1

Take a look at the [collatz conjecture on wikipedia](https://en.wikipedia.org/wiki/Collatz_conjecture) if you would like to read more about it.


Exercise 4
---

Write a program that takes a phrase and prints it reversed.

[Bonus]: if it is a palindrome, output a sentnce saying so.

Example 1:

> Enter a phrase: **Andre Castro**<br>
> ortsaC erdnA

Bonus Example:

> Enter a phrase: **lionoil**<br>
> lionoil<br>
> lionoil is a palindrome!


Exercise 5
---

Password-protect one of the previous exercises from this lab.
The user gets at least 5 attempts to guess the password before the program quits with a failure message.
The maximum number of tries is up to you.
Read a single word as the password.
Output a hint if the user gets it wrong.

[Bonus]: treat words with lowercase and uppercase letters the same.
 For instance, ``WorD`` and ``woRd`` should both be considered correct.

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
[quiz04](https://goo.gl/forms/NWbZ5G4ZiYieqh2B3)

