Note
---

You do not need to complete bonus exercises.
I recommend you attempt them, but if you are spending too long move to the next exercise.


Exercise 1
---

Get a word from the user and print it back.
Each print should have one less letter than the line before it.
Stop printing when there are no more characters in the string.

[Bonus 1]: Get an entire line of text from the user.

[Bonus 2]: Skip an extra amount for spaces you encounter.
Read [this](https://zybooks.zyante.com/#/zybook/UCRCS10Fall2016/chapter/8/section/3) (warning: advanced), and checkout the bonus example below.

Example:

> Enter a string: **Test**</br>
> Test </br>
> Tes </br>
> Te </br>
> T

Bonus 2 Example:

> Enter a string: **Hey there!**</br>
> Hey there</br>
> Hey ther</br>
> Hey the</br>
> Hey th</br>
> Hey t</br>
> Hey</br>
> He</br>
> H</br>

An **incorrect** version of bonus 2:

> Enter a string: **Hey there!**</br>
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

Get two integers from the user and multiply them without using the ``*`` operator.

Example:

> Enter two numbers: **5 6**</br>
> 5 * 6 = 30


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

Write a program that takes a string and reverses it.

[Bonus]: if it is a palindrome, output a sentnce saying so.

Example 1:

> Enter a string: **Andre Castro**<br>
> ortsaC erdnA

Bonus Example:

> Enter a string: **lionoil**<br>
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
[quiz03]()

