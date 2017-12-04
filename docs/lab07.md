Tips
---

Once you complete a function, you can use it in later exercises.

We have written some unit tests for you to use.
There are two ways you can get them into your workspace.

**Method 1**:
Run this command in your terminal where you would like to place ``tests.cpp``.

```sh
wget https://raw.githubusercontent.com/cs-si-ucr/cs10tests/master/week07/tests.cpp
```

**Method 2**:
Go <a href="https://github.com/cs-si-ucr/cs10tests/tree/master/week07" target="_blank">here</a> and download ``tests.cpp`` to your workspace.

In both cases, make sure ``tests.cpp`` is in the same directory as your other code from this week.

Use this as a guide for starting your lab this week:

```cpp
#include "tests.cpp"

using namespace std;

// this is function stubbing:
// they will compile and run, but not produce the correct result.
// that is not the point.
// the point is to get everything to compile.

int myMax(int left, int right) {
    return 0;
}

int myMin(int left, int right) {
    return 0;
}

int myAbs(int n) {
    return -1;
}

double myFabs(double n) {
    return -1.0;
}

int modInt(int numerator, int denominator) {
    return -1;
}

double modDouble(double numerator, double denominator) {
    return -1.0;
}

// TODO: stub the rest of the functions

int main() {
    // to run all tests:
    runAllTests();
}
```


Exercise 1
---

Write a function that returns the ``max`` of two integers.
Call it ``myMax``.


Exercise 2
---

Write a function that returns the ``min`` of two integers.
Call it ``myMin``.


Exercise 3
---

Write a function that returns the absolute value of an integer.
Call it ``myAbs``.


Exercise 4
---

Write a function that returns the absolute value of a floating-point number.
Call it ``myFabs``.


Exercise 5
---

Write a function that returns the ``modulo`` of two integers.
Do not use the ``%`` operator.
Call it ``modInt``.


Exercise 6
---

Write a function that returns the ``modulo`` of two floating-point numbers.
Call it ``modDouble``.


Exercise 7
---

Write the ``isUpper`` function.
``isUpper`` returns true if it is passed an uppercase character.
Call it ``myIsUpper``.


Exercise 8
---

Write the ``isLower`` function.
``isLower`` returns true if it is passed a lowercase character.
Call it ``myIsLower``.


Exercise 9
---

Write the ``isDigit`` function.
``isDigit`` returns true if it is passed a numeric character.
Call it ``myIsDigit``.


Exercise 10
---

Write the ``isAlpha`` function.
``isAlpha`` returns true if it is passed an alphabetic character.
Call it ``myIsAlpha``.


Exercise 11
---

Write the ``isAlnum`` function.
``isAlnum`` returns true if it is passed an alphabetic character *or* a numeric character.
Call it ``myIsAlnum``.


Exercise 12
---

Write the ``toupper`` function.
Call it ``myToUpper``.


Exercise 13
---

Write the ``tolower`` function.
Call it ``myToLower``.


Exercise 14
---

Write a function that accepts an integer and a character.
The function should print the character the number of times passed into it.
Call it ``printRow``.

**Note**: This function cannot be tested by ``tests.cpp``.
You will need to check it yourself.


Exercise 15
---

Write a floating-point comparison function.
Remember that floating-point values are not always stored perfectly precisely.
The function should accept two doubles to compare, along with a tolerance value.
The tolerance specifies how much of a difference between two numbers there can be while still considered to be equal.
The difference should be strictly less than the tolerance value.

Call it ``flEq``.


Exercise 16
---

Write a function that returns a random number in a specified range.
Call it ``randRange``.


Exercise 17
---

Write a function that returns the first index of a character in a provided string.
Return ``-1`` if the character is unable to be found.
Call it ``findCharBegin``.


Exercise 18
---

Write a funciton that returns the first index of a string in a provided string.
Return ``-1`` if the string is unable to be found.
Call it ``findStringBegin``.


Exercise 19
---

Write a function that returns the index of a character in a provided string given a starting location.
Return ``-1`` if the character is unable to be found.
Call it ``findChar``.


Exercise 20
---

Write a funciton that returns the index of a string in a provided string given a starting location.
Return ``-1`` if the string is unable to be found.
Call it ``findString``.


