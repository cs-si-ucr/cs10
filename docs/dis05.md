Introduction
---

A loop that appears in the body of another loop is often called a
<a style="color:white;border:solid black;border-width:1px">nested loop</a>.

The loops on the inside of a nested loop construct are called
<a style="color:white;border:solid black;border-width:1px">inner loops</a>
while the loop on the outside of a nested loop construct is called the
<a style="color:white;border:solid black;border-width:1px">outer loop</a>

Building a complex program by making small testable additions and changes is called 
<a style="color:white;border:solid black;border-width:1px">incremental programming</a>

A loop construct that executes the body of the loop before checking the loop condition is called a
<a style="color:white;border:solid black;border-width:1px">do-while loop</a>

Debugging Practice
---

The code below is supposed to continuously ask the user for a number and output the square of that number.
When the user enters 0 the program should exit.
Unfortunately, the program below does not even compile, although thats not the only problem...

How can you modify the following code so that it works correctly?

```c++
#include <iostream>

using namespace std;

int main() {
    int userInput = 0;

    do {
        cout << "Enter a number: ";
        cin >> input;
        cout << endl;

        cout << input << " * " << input << " == " << input * input << endl; 

    } while (input > 0)
    
    return 0;
}
```

The code below is supposed to output a word diagonally, but it does not seem to be working.

For example, when the user inputs "hey" the output should be:

h<br>
&nbsp;&nbsp;e<br>
&nbsp;&nbsp;&nbsp;&nbsp;y<br>

But instead the output is:

h&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y 

How can you modify the following code so that it works correctly?

```c++
#include <iostream>

using namespace std;

int main() {
    string userInput;

    cout << "Enter a string: ";
    getline(cin, userInput);
    cout << endl;

    for (int i = 0; i < userInput.size(); i++) {
        for (int j = 0; j < userInput.size(); j++) {
            if (i == j) {
                cout << userInput.at(i);
            }
            else {
                cout << ' ';
            }
        }
    }
    return 0;
}
```

Code Tracing
---

For the code below answer the following questions.

1. What does this program output?
2. What would happen if you switched the values of width and height? (That is, `width = 13;` and `height == 2;`)

```c++
int main(){
    char start = 'a';
    int width = 2;
    int height = 13;

    for (int i = 0; i < height; i++) {
        for (int j = 0; j < width; j++) {
            cout << start << ' ';
            start++;
        }
        cout << endl;
    }

    return 0;
}
```

For the code below answer the following questions.

1. What does the code output if the user enters 2. What about if the user enters a 3 or a 4? That is, what does the main function output in the seperate cases of `userInput == 2`, `userInput == 3`, and `userInput == 4`.
2. What mathematical function does each part represent? (refer to the comments in the code if you are unsure what is meant by 'part')
3. What mathematical function would we have if we incremented the variable `result` in *n* nested for-loops?

```c++
int main() {
    int userInput = 0;

    cout << "Enter a number: ";
    cin >> userInput;
    cout << endl;

    //PART 1
    int result = 0;

    for (int i = 0; i < userInput; i++) {
        result++;
    }

    cout << result << endl;

    //PART 2
    result = 0;

    for (int i = 0; i < userInput; i++) {
        for (int j = 0; j < userInput; j++) {
            reuslt++;
        }
    }

    cout << result << endl;
    
    //PART 3 
    result = 0;

    for (int i = 0; i < userInput; i++) {
        for (int j = 0; j < userInput; j++) {
            for (int k = 0; k < userInput; k++) {
                result++;
            }
        }
    }

    cout << result << endl;
    result = 0;

    return 0;
}
```
