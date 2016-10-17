
Introduction
---

Strings can be compared for equality by using the
<a style="color:white;border:solid black;border-width:1px">== or !=</a>operators .</br>
For two strings to be considered equal, they must have the same number of
<a style="color:white;border:solid black;border-width:1px">characters</a>
and the same characters in the same
<a style="color:white;boreder:solid black;border-width:1px">order.</br>

<a style="color:white;border:solid black;border-width:1px"><,>,<=,>=</a>
can also be used to compare strings based off thier
<a style="colo:white;border:solid black;border-wiodth:1px">ASCII values.</br>

The string accessor functions ``.at(i)`` returns
<a style="color:white;border:solid black;border-width:1px">a character</a>
at the ith value of the string. </br>
The string accessor function ``.length()`` returns
<a style="color:white;border:solid black;border-width:1px">the number of chars in the string</a>
or the length of the string.</br>
``substr(i,j)`` would split a string into a substring from position
<a style="color:white;border:solid black;border-width:1px">i</a>
and until position
<a style="color:white;border:solid black;border-width:1px">i+j</a></br>

``.toupper('c')`` and ``.tolower('C')`` are char functions that return the
<a style="color:white;border:solid black;border-width:1px">lower and uppercase</a>
of the chars pased in respectively.</br>

Floating point numbers should not be compared using ``==`` because they are not always so 
<a style="color:white;border:solid black;border-width:1px">precise</a>.</br>
Instead, to compare to floating point variables ``f1`` and ``f2``, make sure to use
<a style="color:white;border:solid black;border-width:1px">(f1-f2)<.00001</a>/</br>

Loops allow you to control the
<a style="color:white;border:solid black;border-width:1px">flow</a>
of your program by repeating a certain code block while 
<a style="color:white;border:solid black;border-width:1px">a certain condition is true</a>.

One type of loop that is similar to an if statement is a 
<a style="color:white;border:solid black;border-width:1px">while</a>
lopo because both contain an expression that evaluates to true/false to enter the loop.</br>
Just like an if statement, a while loops conditional statment must evaluate to
<a style="color:white;border:solid black;border-width:1px">true</a>
in order to enter the code block.</a>

A while loop will continue to run until
<a style="color:white;border:solid black;border-width:1px">its conditional statment is false</a>.
However, since this condition is only checked at the
<a style="color:white;border:solid black;border-width:1px">beginning</a>
of each loop iteration, even if the statement becomes false during the execution of the loop, the while loop will continue to run.

<a style="color:white;border:solid black;border-width:1px">For</a>
loops are another kind of loop.</br>
Rather than havine one conditional statement, a for loop is composed of
<a style="color:white;border:solid black;border-width:1px">3</a>
parts.</br>
* 1) Initializing a
<a style="color:white;border:solid black;border-width:1px">variable</a>.</br>
* 2) Like while loops, the
<a style="color:white;border:solid black;border-width:1px">conditional statement</a>
or the loop expression.</br>
* 3) And lastly, the loop variable
<a style="color:white;border:solid black;border-width:1px">update</a>.

Although both for and while loops each can perform the same tasks, they should be used for different purposes.</br>
A for loop should be used when the amount of loop iterations is
<a style="color:white;border:solid black;border-width:1px">known</a></br>
while a while loop should be used when iteration should occur until a certain condition is
<a style="color:white;border:solid black;border-width:1px">false</a>.

Code tracing
---

What does each main function ouptut?
Assume all required libraries are included.
Refer to the next section for extra help.

```c++
// 1
int main(){
    string Z = "Z";
    string a = "a";
    
    if(Z < a){
        cout << "Z comes before a alphabetically" << endl;
    }
    else{
        cout << "a comes before z alphabetically" << endl;
    }
    
    Z.append("ebra");
    cout << "Length = " << Z.length() << endl;
    
    Z.clear();
    cout << "Length = " << Z.length() << endl;
    
    Z = "hello";
    cout << Z.at(0) << a << Z.at(2) << Z.at(4) << endl;
    
    Z.insert(0,"c");
    cout << Z << endl;
    
    cout << Z.substr(1,2) << " is awesome." << endl;
    
    return 0;
}

// 2
int main(){
    int counter = 0;
    int counter2 = 0;
    
    for(int i = 0; i < 5; i++){
        counter += 1;
    }
    cout << counter << endl;
    
    for(int i = 0; i < 4; i++){
        counter *= 2;
    }
    cout << counter << endl;
    
    counter = counter / 10;
    
    for(int i = 28; i > counter; i = i-2){
        cout << counter2;
        counter2++;
    }
    cout << endl;
    
    return 0;
}

// 3
int main(){
    bool b = true;
    int a = 0;
    
    while(b){
        cout << a;
        if(a == 5){
            b = false;
        }
        a++;
    }
    cout << endl;
    
    b = true;
    a = 0;
    
    while(b){
        a++;
        if(a == 5){
            b = false;
        }
        cout << a;
        cout << endl;
    }
    
    double d = 12345;
    
    while(d >= 1){
        d = d / 10;
    }
    cout << d << endl;
    
    string s = "Computer";
    
    while(s.length() != 0){
        cout << s << endl;
        s.resize(s.length()-1);
    }
    
    return 0;
}

// 4
// FOR THESE QUESTIONS, how many times does each loop run?
int main(){
    for(int i = 0; i < 10; i++){
        if(i < 5){
            i *= 2;
        }
    }
    
    int j = 10;
    
    while(j != 0){
        if(j > 0){
            j -= 3;
        }
        if(j < 0){
            j += 5;
        }
    }
    
    
    for(int i = 0; i < 30; i ++){
        if(i%3 == 2){
            i += 10;
        }
        else if(i%3 == 1){
            i *= 2;
        }
        else{
            i /= 3;
        }
    }
    
    
    return 0;
}
```

Extra Help
---

* [ASCII Table](http://www.asciitable.com/)
