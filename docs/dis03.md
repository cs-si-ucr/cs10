Introduction
---

A variable of ``char`` type can store a
<a style="color:white;border:solid black;border-width:1px">single character</a>.</br>
Character literals must be declared using
<a style="color:white;border:solid black;border-width:1px">single quotes</a>.</br>
<a style="color:white;border:solid black;border-width:1px">ASCII</a>
is a standard for encoding characters to numbers.</br>
An
<a style="color:white;border:solid black;border-width:1px">escape sequence</a>
is a two-character sequence that represent a special character. Example: ``'\n'``

An initialized variable whose value cannot change is called a </br>
<a style="color:white;border:solid black;border-width:1px">constant variable</a>.

An 
<a style="color:white;border:solid black;border-width:1px">overflow</a>
occurs when the value being assigned to a variable is greater than the maximum value the variable can store.

When debugging error messages from compilation, start from the
<a style="color:white;border:solid black;border-width:1px">top</a>
of the error messages and work 
<a style="color:white;border:solid black;border-width:1px">down</a>
recompiling after each message.

A ``bool`` stores a
<a style="color:white;border:solid black;border-width:1px">true\\false value</a>.

<a style="color:white;border:solid black;border-width:1px">Braces \{\}</a>
surround a branch's statements.</br>
<a style="color:white;border:solid black;border-width:1px">Parentheses \(\)</a>
surround a branch's conditions.</br>
If-else statements within other if/else statements are called: </br>
<a style="color:white;border:solid black;border-width:1px">nested if-else statements</a>.

The 6 relational and equality operators are:
<a style="color:white;border:solid black;border-width:1px"><, >, <=, >=, ==, \!=</a>.</br>
These relational operators evaluate to a
<a style="color:white;border:solid black;border-width:1px">boolean value</a>.

The 3 logical operators are:
<a style="color:white;border:solid black;border-width:1px">&&, ||, \!</a>.</br>
``&&`` is true when 
<a style="color:white;border:solid black;border-width:1px">both of its operands are true</a>.</br>
``||`` is true when
<a style="color:white;border:solid black;border-width:1px">at least one of its operands are true</a>.</br>
``!`` is true when
<a style="color:white;border:solid black;border-width:1px">its operand is false</a>.

The order of evaluation for logical/relational operators is: </br>
<a style="color:white;border:solid black;border-width:1px">\(\)</a>
,
<a style="color:white;border:solid black;border-width:1px">\!</a>
,
<a style="color:white;border:solid black;border-width:1px">\* \\ % \+ \-</a>
,
<a style="color:white;border:solid black;border-width:1px">< <= > >=</a>
,
<a style="color:white;border:solid black;border-width:1px">== \!=</a>
,
<a style="color:white;border:solid black;border-width:1px">&</a>
,
<a style="color:white;border:solid black;border-width:1px">|</a>
,
<a style="color:white;border:solid black;border-width:1px">&&</a>
,
<a style="color:white;border:solid black;border-width:1px">||</a>

Code tracing
---

What does each main function ouptut?
Assume all required libraries are included.
Refer to the next section for extra help.

```c++
// 1
int main() {
    char c1 = 'a';
    char c2 = c1 - 32;
    
    cout << c1 << ' ' << c2 << endl;
    
    c1 += 1;
    c2 += 1;
    
    cout << c1 << ' ' << c2 << endl;
    
    return 0;
}

// 2
int main() {
    int i = 2;
    int j = 5;
    int k = -3;
    
    if(i > k) {
        i *= k;
    }
    
    if (j < i) {
        j *= i;
    }
    else {
        j /= 5;
    }
    
    if (j * 3 > -k) {
        k = -k / 3;
    }
    else if (j * 3 <= -k) {
        j = j * 3;
        k = -k;
    }
    
    if (i > 0) {
        i = k;
    }
    else if (k > 0) {
        k = i;
    }
    else if (j > 0) {
        j = i;
    }
    
    cout << "i = " << i << endl;
    cout << "j = " << j << endl;
    cout << "k = " << k << endl;
    
    return 0;
}

// 3
int main() {
    int i = 2;
    int j = 5;
    int k = -3;
    bool b1 = true;
    
    if (i > k && !b1) {
        i *= k;
    }
    
    if (j < i && b1) {
        j *= i;
    }
    else {
        j /= 5;
    }
    
    if (!(j * 3 > -k)) {
        k = -k / 3;
    }
    else if (j * 3 <= -k) {
        j = j * 3;
        k = -k;
    }
    
    if (!(i > 0) || (j - i > 0)) {
        i = k;
    }
    else if (((k > 0) && !(-k < 0)) || b1) {
        k = i;
    }
    else if (!(j > 0) || (i - j > 0)) {
        j = i;
    }
    
    cout << "i = " << i << endl;
    cout << "j = " << j << endl;
    cout << "k = " << k << endl;

    return 0;
}

// 4
int main() {
    int i = 2;
    int j = 5;
    int k = -3;
    bool b1 = true;
    
    if (i > k && b1) {
        if (-i < -k || !b1) {
            k += 5;
        }
        i *= k;
    }
    
    if (j >= i) {
        if (j == i) {
            j -= 6;
        }
        j /= i;
    }
    else {
        if (j > k && j < i) {
            j -= 1;
        }
        j *= 5;
    }
    
    if (j * 3 > k) {
        if (!(j * 3 <= -k)) {
            b1 = !b1;
        }
        k = -k * 3;
    }
    else if (j * 3 <= -k || b1) {
        j = j * 3;
        k = -k;
    }
    
    if (!(i > 0) || (j - i > 0)) {
        i = k;
        if (i == k) {
            k += 6;
        }
    }
    else if (((k > 0) && !(-k < 0)) || b1) {
        k = i;
        if (b1) {
            i += 6;   
        }
    }
    else if (!(j > 0) || (i - j > 0)) {
        j = i;
        if (b1) {
            j += 6;
        }
        else if (b1 || !b1) {
            i += 3;
        }
    }
    
    cout << "i = " << i << endl;
    cout << "j = " << j << endl;
    cout << "k = " << k << endl;

    return 0;
}
```

Extra Help
---

* [ASCII Table](http://www.asciitable.com/)
