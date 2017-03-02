# Introduction

A
<a style="color:white;border:solid black;border-width:1px">function</a>
is a named block of code.
Invoking a function name, also known as a
<a stlye="color:white;border:solid black;border-width:1px">function call</a>
causes the functions statements to execute.

A function
<a style="color:white;border:solid black;border-width:1px">declaration</a>
consists of a new function name, its return type, and its parameter list.
It is optionally followed by a block of statements.
Including the statements is called
<a style="color:white;border:solid black;border-width:1px">definition</a>.

In the statement `void print(string strName);`
`strName` is a
<a style="color:white;border:solid black;border-width:1px">parameter</a>.
A function may have multiple parameters, seperated by
<a style="color:white;border:solid black;border-width:1px">commas</a>.
A function without parameters must still have parenthesis. 
The value passed to a parameter is kmown as an
<a style="color:white;border:solid black;border-width:1px">agrument</a>.

Each non-void function must have a
<a style="color:white;border:solid black;border-width:1px">return</a>
statement which tranfers control of the program back to the where the functions was originally called.

The return value of a function depends on how the function is declared.
For example, in the function `int main()` a function named `main` is declared to have a return type of 
<a style="color:white;border:solid black;border-width:1px">int</a>.
If a function is declared to be `void` as it is in the `print` example above, then the return statement should simply be 
<a style="color:white;border:solid black;border-width:1px">return;</a>,
or could be left out entirely.

Designating blocks of codes as functions can be useful for three reasons:

1. Improving program
<a style="color:white;border:solid black;border-width:1px">readability</a>

2. <a style="color:white;border:solid black;border-width:1px">Modular</a>
program development </br>

3. Avoiding
<a style="color:white;border:solid black;border-width:1px">redundant</a>
code


# Code Tracing

What do the following programs output?

###### 1

```c++
void foo(int a, int b) {
    a += 6;
    b += a;
    b = a * b;
    a = a + b;
    cout << a << endl;
    cout << b << endl;
}

int main() {
    int a = 5;
    int b = 3;
    cout << "Functions" << endl;
    foo(a,b);
    cout << "take parameters." << endl;

    return 0;
}
```


##### 2

```c++
void printa() {
    cout << "the bomb" << endl;
}
void printb() {
    cout << "dot com" << endl;
}

void foo(int a) {
    if (a < 5) {
        printa();
    } else if (a == 5) {
        printb();
    } else {
        cout << "none" << endl;
    }
}

int main() {
    int a = 5;
    int b = -5;
    foo(a);
    foo(b);

    return 0;
}
```


##### 3

```c++
int foo2(int b) {
    int c = b + 6;
    if (c > 13) {
        b = b + 5;
    } else {
        b = b + 9;
    }
    
    return c + b;
}

int foo(int a) {
    if (a > -1) {
        return -1;
    } else if (a < 0) {
        return 0;
    }
}

int main() {
    int a = 0;
    int b = 7;
    if (foo(a) == 1) {
        cout << "Positive!" << endl;
    } else {
        cout << "Negative!" << endl;
    }

    cout << foo2(b) + foo(a) << endl;

    return 0;
}
```


##### 4

```c++
int getSize(string t) {
    return t.size();
}

string removeCaps(string text) {
    for (int i = 0; i < text.size(); i++) {
        if (text.at(i) == 's' || text.at(i) == 'S') {
            cout << "S found!" << endl;
            text.replace(i, 1, "");
        }
    }
    return text;
}

int main() {
    string text = "StephenStrange";
    string modifiedText = removeCaps(text);
    if (getSize(modifiedText) < getSize(text)) {
        cout << "Made at least one change to text!" << endl;
    } else {
        cout << "Made no changes to text." << endl;
    }
    cout << modifiedText << endl;
}
```
