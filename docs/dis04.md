Introduction
---

You can compare two strings for similarity using the
<a style="color:white;border:solid black;border-width:1px">==</a>
or
<a style="color:white;border:solid black;border-width:1px">==</a>
operator.
For two strings to be considered equal, they must have the same number of
<a style="color:white;border:solid black;border-width:1px">characters</a>
and each corresponding character must be
<a style="color:white;border:solid black;border-width:1px">identical</a>.

The operators
<a style="color:white;border:solid black;border-width:1px"><, <=, >, >=</a>
can also be used to order strings 
<a style="color:white;border:solid black;border-width:1px">values</a>.

The string accessor function ``.at(i)`` returns
<a style="color:white;border:solid black;border-width:1px">a character</a>
at the ith value of the string
The string accessor function ``.size()`` returns
<a style="color:white;border:solid black;border-width:1px">the number of chars in the string</a>
or the length of the string.
``substr(i,j)`` would split a string into a substring from index
<a style="color:white;border:solid black;border-width:1px">i</a>
and until index
<a style="color:white;border:solid black;border-width:1px">i+j</a></br>

``toupper('c')`` and ``tolower('C')`` are char functions that return the
<a style="color:white;border:solid black;border-width:1px">lowercase and uppercase</a>
of the character arguments, respectively.

Floating point numbers should not be compared using ``==`` because they are sometimes not
<a style="color:white;border:solid black;border-width:1px">precise</a>
enough.
Instead, to compare to floating point variables ``f1`` and ``f2`` where ``f1 > f2``, make sure to use a formula similar to the following:
<a style="color:white;border:solid black;border-width:1px">(f1-f2)<.00001</a>.

Loops allow you to control the
<a style="color:white;border:solid black;border-width:1px">flow</a>
of your program by repeating actions.
Each loop style contains a condition section.
The block will execute as long as the provided condition evaluates to
<a style="color:white;border:solid black;border-width:1px">true</a>.

One type of loop that is visually similar to an ``if`` statement is a 
<a style="color:white;border:solid black;border-width:1px">while</a>
loop.
Both contain a single expression that evaluates to ``true`` or ``false``.
This expression determines whether or not the body of the loop will be
<a style="color:white;border:solid black;border-width:1px">executed</a>.

A while loop will continue to execute until
<a style="color:white;border:solid black;border-width:1px">its conditional expression evaluates to false</a>.
The condition of a while loop evaluates once per iteration of the loop.

``for`` loops are similar to ``while`` loops.
For loops are composed of
<a style="color:white;border:solid black;border-width:1px">an initialization statement</a>,
<a style="color:white;border:solid black;border-width:1px">a conditional expression</a>, and
<a style="color:white;border:solid black;border-width:1px">an update action</a>.
The conditional expression of a ``for`` loop is evaluated
<a style="color:white;border:solid black;border-width:1px">before</a>
the body is executed.

Although ``for`` and ``while`` loops can be used interchangeably, each is stylistically better suited for different tasks.
A ``for`` loop should be used when the number of loop iterations is
<a style="color:white;border:solid black;border-width:1px">known</a>.
A ``while`` loop should be used when the number of loop iterations is
<a style="color:white;border:solid black;border-width:1px">unknown</a>.

Code tracing
---

What does each main function ouptut?
Assume all required libraries are included.

```c++
// 1
int main() {
    string Z = "Z";
    string a = "a";
    
    if (Z < a) {
        cout << "'Z' comes before 'a' lexicographically" << endl;
    }
    else {
        cout << "'a' comes before 'Z' lexicographically" << endl;
    }
    
    Z.append("ebra");
    cout << "Length = " << Z.length() << endl;
    cout << "Size = " << Z.size() << endl;
    
    Z.clear();
    cout << "Length = " << Z.size() << endl;
    
    Z = "hello";
    cout << Z.at(0) << a << Z.at(2) << Z.at(4) << endl;
    
    Z.insert(0,"c");
    cout << Z << endl;
    
    cout << Z.substr(1,2) << " is awesome." << endl;
    
    return 0;
}

// 2
int main() {
    int counter = 0;
    int counter2 = 0;
    
    for (int i = 0; i < 5; i++) {
        counter += 1;
    }
    cout << counter << endl;
    
    for (int i = 0; i < 4; i++) {
        counter *= 2;
    }
    cout << counter << endl;
    
    counter = counter / 10;
    
    for (int i = 28; i > counter; i = i - 2) {
        cout << counter2;
        counter2++;
    }
    cout << endl;
    
    return 0;
}

// 3
int main() {
    bool b = true;
    int a = 0;
    
    while (b) {
        cout << a;
        if (a == 5) {
            b = false;
        }
        a++;
    }
    cout << endl;
    
    a = 0;
    
    while (!b) {
        a++;
        if (a == 5){
            b = true;
        }
        cout << a << endl;
    }
    
    double d = 12345;
    
    while (d >= 1) {
        d = d / 10;
    }
    cout << d << endl;
    
    string s = "Computer";
    
    while(s.size() != 0) {
        cout << s << endl;
        s.resize(s.size() - 1);
    }
    
    return 0;
}

// 4
// FOR THESE QUESTIONS, how many times does each loop run?
int main() {
    // Loop A
    for (int i = 0; i < 10; i++) {
        if (i < 5) {
            i *= 2;
        }
    }

    int j = 10;
    
    // Loop B
    while (j != 0) {
        if (j > 0) {
            j -= 3;
        }
        if (j < 0) {
            j += 5;
        }
    }

    // Loop C
    for (int i = 0; i < 30; i++) {
        if (i % 3 == 2) {
            i += 10;
        }
        else if (i % 3 == 1) {
            i *= 2;
        }
        else {
            i /= 3;
        }
    }

    return 0;
}
```
