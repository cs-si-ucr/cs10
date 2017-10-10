Lab 2 Solutions
---

This page is for reference only. It is intended to be viewed after you finish your in-lab assignments.


Exercise 1
---

Ask the user for 2 numbers, then divide them and show the result.

Example:

> Enter the dividend: <u>**4**</u><br>
> Enter the divisor: <u>**2**</u><br>
> 4 / 2 == 2

```
#include <iostream>
using namespace std;

int main() {
    cout << "Enter the dividend: ";
    
    int dividend;

    cin >> dividend;

    cout << "Enter the divisor: ";

    int divisor;

    cin >> divisor;

    cout << dividend << " / " << divisor << " == " << dividend / divisor << endl;

    return 0;
}
```

Exercise 2
---

Get a character from the user, and display its integer equivalent.
The keyword for the character datatype is ``char``.

Example:

> Enter a character: <u>**c**</u><br>
> 'c' in decimal is 99.

<!-- todo: delete -->

```
#include <iostream>
using namespace std;

int main() {
    char userInput;
    
    cout << "Enter a character: " << endl;

    cin >> userInput;

    cout << "'" << userInput - '0' << endl;
    
    return 0;
}
```

Exercise 3
---

Get a 5-character word from the user.
Convert it to the "proper" capitalization (first letter is capitalized, and the rest are lowercase).

Example:

> Enter a 5-character word: <u>**hElLo**</u><br>
> Your word is Hello.


Exercise 4
---

Write a program to perform modulus between two floating-point values.
The modulus operator `%` will not work on doubles.
Do not use `fmod` from the cmath library (although you can use it to verify your results).
Do not worry about negative values or modding by 0.


Here is a hint:

> For two positive integers N (numerator) and D (denominator),<br>
> N can be expressed as D\*m + R.<br>
> m is some integer multiple of D.<br>
> R is the remainder of the division between N and D.<br>
> R = N - D*m<br>
> R and m are unknowns in this equation.<br>
> Find m to solve for R.

Examples:

> Enter the dividend: <u>**23.4**</u><br>
> Enter the divisor: <u>**3.2**</u><br>
> 23.4 % 3.2 == 1

> Enter the dividend: <u>**54.7**</u><br>
> Enter the divisor: <u>**3.14**</u><br>
> 54.7 % 3.14 == 1.32


Exercise 5 (advanced)
---

Use modulus and division to print the binary value of a character.

Example:

> Enter a character: <u>**c**</u><br>
> 'c' in binary is 01100011.

Hint: once you have the decimal value of a character [part 3],
you can google something like "<a href="http://lmgtfy.com/?q=99+in+binary" target="_blank">99 in binary</a>"
to double-check your results.
Also, characters all have 8 bits.




<!-- future idea: give them some poorly-formatted code and have them format it properly.
     It could do anything, because they don't need to understand it to format it. -->



Quiz!
---
[quiz02](https://docs.google.com/a/ucr.edu/forms/d/e/1FAIpQLSfg05rmW2RMtUtPpVbj4uME7MCHdHpqH_qYJ4EFRNeoFGA3Dw/viewform)


