Introduction
---

A variable is a
<a style="color:white;border:solid black;border-width:1px">named location in memory</a>.
The name we give a variable is called an
<a style="color:white;border:solid black;border-width:1px">identifier</a>.

Variables can be assigned to using the
<a style="color:white;border:solid black;border-width:1px">=</a> operator.

In c++, ``* / % + -`` are mathematical operators, and can be used to
<a style="color:white;border:solid black;border-width:1px">multiply</a>,
<a style="color:white;border:solid black;border-width:1px">divide</a>,
<a style="color:white;border:solid black;border-width:1px">modulo</a>,
<a style="color:white;border:solid black;border-width:1px">add</a>, and
<a style="color:white;border:solid black;border-width:1px">subtract</a> two numbers, respectively.

c++ math operators behave according to precedence.
<a style="color:white;border:solid black;border-width:1px">(&nbsp;)</a>
has the highest precedence.
Next is
<a style="color:white;border:solid black;border-width:1px"> \* / % </a>,
and they have the same precedence.
Last are
<a style="color:white;border:solid black;border-width:1px">+</a>
and
<a style="color:white;border:solid black;border-width:1px">-</a>;
They have the same precedence.

When an expression has multiple operators of the same precedence, they are evaluated
<a style="color:white;border:solid black;border-width:1px">left to right</a>.
For instance, 4/1/2==(4/1)/2, and **not** 4/(1/2).
<a style="color:white;border:solid black;border-width:1px">(the second would be a problem)</a>


Arithmetic expressions don't always behave the way they do in math.
In math, 3/4==0.75 .
In c++, 3/4==<a style="color:white;border:solid black;border-width:1px">0</a>.
Division is the only operator that doesn't play nice.
The next most common integer arithmetic mistake is with precedence.
This can be avoided by using parenthesis, in most cases.

Because ``int`` only stores
<a style="color:white;border:solid black;border-width:1px">integers</a>,
all fractional information is lost.
If you want to do math with fractional information included, use
<a style="color:white;border:solid black;border-width:1px">double</a>.

The ``string`` is used to store text information.
A string can be thought of as a collection of
<a style="color:white;border:solid black;border-width:1px">characters</a>.

Lastly, and most importantly, 
<a style="color:white;border:solid black;border-width:1px">**FOLLOW THE STYLE GUIDELINES**</a>.


Code tracing
---

What does each main function ouptut?
Assume all required libraries are included.
Refer to the next section for extra help.

```c++
// 1
int main() {
    int temp = 4;
    double temp2 = 2.5;
    float temp3 = 2.0;

    cout << temp3 << endl;
    cout << temp/ temp2 << endl;

    temp = temp2;
    cout << temp << endl;

    return 0;
}

// 2
int main() {
    int temp = 4;
    double temp2 = 2.5;
    double temp3 = 1.5;

    temp3 = temp / temp2;
    temp /= temp2;

    cout << temp3 << ", " << temp << endl;

    // some other primitive number variable types:
    float temp4 = 5.5;     // half the precision of double
    long temp5 = 9.1;
    short temp6 = 4.7;
    long long temp7 = 8.6;

    cout << temp4 + temp6 << endl;
    temp7 -= temp5;
    cout << temp7 << endl;

    return 0;
}

// 3
int main() {
    string jake = "jake";
    string james = "james";
    char a = 'a';

    jake = james;
    cout << jake << endl;
    jake = jake + james;
    cout << jake << endl;

    jake = "j";
    jake += a;
    a += 12;
    jake += a;
    a -= 8;
    jake += a;
    a = ((a/ 2) * 3) - (12*2 + 4); // hint: http://www.ascii-code.com/
    jake += a;
    cout << jake << endl;

    return 0;
}

// 4
int main() {
    int intgr = 20;
    char letter = 'a';
    double dbl = 10.67;

    cout << static_cast<char>(letter + static_cast<int>(dbl) * 2 - intgr * 2.5);
    cout << static_cast<char>((intgr * 2 + dbl * 4) + (dbl / 9));
    cout << " " << intgr % 11 + 1;
    string temp = "";
    temp += static_cast<char>(intgr + 12);
    temp += static_cast<char>(letter + static_cast<int>(dbl) - 1.67);
    temp += (18+ letter);
    cout << temp << " awesome!" << endl;

    return 0;
}
```


Extra Help
---

* [type conversion specifics:](http://www-h.eng.cam.ac.uk/help/tpl/languages/C++/strongtyping.html)
* [standard math library](http://www.cplusplus.com/reference/cmath/)
* the space character ``' '`` has an value of 32


