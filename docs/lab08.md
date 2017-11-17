# Instructions

Complete exercises 1 through 4 in groups of 2 or more.
One or more people will solve the problems.
The rest (minimum of 1) of the group will write the test cases.
This should alternate per exercise.

You are allowed to use assert in your tests.


# Exercise 1

Write a function that orders two integers.
The first passed in should be set to the least of the two.
The second passed in should be set to the greatest of the two.

Example:

```c++ 
// in main
int a = 5;
int b = 4;
foo(a, b);
cout << a << endl;
cout << b << endl;
```

> should result in an output of: <br>
> 4<br>
> 5


# Exercise 2

Write 4 different swap functions.
Each swap function accepts two reference parameters, and swaps them.
The 4 swap functions should operate on ``int``, ``double``, ``char``, and ``bool``.

We will name them all the same thing: ``swap``.
This takes advantage of overloading.
Overloading is when two functions have the same name, but different **parameter lists**.

Example:
```c++
int main() {
	char a = 'a';
	char c = 'c';
	swap(a, c);
	
	int one = 1;
	int two = 2;
	swap(one, two);

	cout << a << " " << b << endl;
	cout << one << " " << two << endl;

	return 0;
}
```

The example above should print:

> c a<br>
> 2 1

`swap(a, c)` and `swap(one, two)` are calls to two different functions, despite having the same name.
Look at the Extra Help section of this page, or ask your SI leader, to learn more about function overloading.


# Exercise 3

Write a function that replaces all occurances of a word with another word.
The function should return an integer indicating how many instances of the word were replaced.

Example:
> Enter a sentence: **the other day my friends and I went to the store to find out the price of radishes**<br>
> Which word should be replaced:  **radishes**<br>
> Replace with what word: **oranges**<br>
> the other day my friends and I went to the store to find out the price of oranges

Example:
> Enter a sentence: **I like to eat apples and bananas but if I am forced to, I will eat just about anything, as long as its not spicy!**<br>
> Which word should be replaced : **eat**<br>
> Replace with what word: **fight** <br>
> I like to fight apples and bananas but if I am forced to, I will fight just about anything, as long as its not spicy!


# Exercise 4

Write a function that modifies a string to contain a subsection of itself.
The function should accept a string, and two integers.
The first integer is where to start the substring from.
The second integer is how many characters to get.

The function should return a bool, signaling whether or not the string was modified.
Do not modify the string if the substr size requested is too big.
Do not modify the string if the starting position is outside the string.

For example, given the following code:

```c++
string str = "Origami";
bool success = substr(str, 1, 3);
if (success) {
    cout << str << endl;
} else {
    cout << "substr failed :(" << endl;
}
```

The output should be:

> rig

Given the following code:

```c++
string str = "Origami";
bool success = substr(str, 5, 3);
if (success) {
    cout << str << endl;
} else {
    cout << "substr failed :(" << endl;
    cout << str << endl;
}
```

The output should be:

> substr failed :(<br>
> origami

# Excercise 5

DO NOT IMPLEMENT THE FUNCTIONS BELOW. READ INSTRUCTIONS.

The code below implements a guessing game.
There are some function headers given to you.
Which parameters should be passed by reference?
The return types of the functions have not been specified. 
What should the return types be?

`generateRand(int)` should generate a random number in the range [1, 20].
This function should not output.

`continuePlaying(string)` prompts the user if they would like to continue playing this game.

The program should continue to run until the user wins, or enters "exit".

Function `playGuessingGame(bool, int, int)` should accept a random number,
and have the user attempt to guess it `maxAttempts` number of times.
If the user correctly guesses the number, the the bool `winStatus` is set to true.
The function then returns the number of tries it took the user to guess the value.

The while loop below does not stop when the user wins.
Fix this.


```c++
// INCORRECT function headers:
generateRand(int);
continuePlaying(string);
playGuessingGame(bool, int, int);

int main(){
	int randInt = 0;
	string userInput;
	bool winStatus = false;
	int numTries = 0;
	int maxAttempts = 3;

	while (userInput != "exit" || !winStatus) {
		generateRand(randInt);
		numTries = playGuessingGame(winStatus, randInt, maxAttempts);
		if (!winStatus) {
			continuePlaying(userInput);
		}
	}

	cout << "It took you " << numTries << "to get the value ";
	if (winStatus) {
		cout << "correct!" << endl;
	} else {
		cout << "incorrect!" << endl;
	}

	return 0;
} 
```
Example:
> A random number has been generated <br>
> What is your guess? (you have 3 attempts remaining): **1**<br>
> INCORRECT!<br>
> What is your guess? (you have 2 attempts remainiing): **2**<br>
> INCORRECT! <br>
> What is your guess? (you have 1 attempt remaining): **12**<br>
> INCORRECT! <br>
> Enter exit if you no longer want to play: **no** <br>
><br>
> A random number has been generated <br>
> What is your guess? (you have 3 attempts remaining): **1**<br>
> CORRECT!<br>
> It took you 1 try to get the value correct!


# Extra Help

* [More on function overloading](http://www.learncpp.com/cpp-tutorial/76-function-overloading/)


# Quiz

[quiz08](https://docs.google.com/a/ucr.edu/forms/d/e/1FAIpQLSc5YyLSWMoNFjj6qm_1otp94c2MafU0ymnWiU-g2ft_Ygu-aQ/viewform)

