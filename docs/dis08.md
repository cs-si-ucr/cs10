Introduction
---
Value parameters receive a
<a style="color:white;border:solid black;border-width:1px">copy</a>
of the argument passed to the function.
Reference parameters receive a 
<a style="color:white;border:solid black;border-width:1px">reference</a>
to the argument passed to the function.

The scope of variables in c++ is from the moment they are
<a style="color:white;border:solid black;border-width:1px">declared</a>
to the
<a style="color:white;border:solid black;border-width:1px">close brace</a>
of the block they were
<a style="color:white;border:solid black;border-width:1px">declared</a>
in.

<a style="color:white;border:solid black;border-width:1px">global variables</a>
can be used in any scope.
They only stop existing when the program ends.
We do not use these in CS10 because it is often bad practice.

A function
<a style="color:white;border:solid black;border-width:1px">prototype</a>
or
<a style="color:white;border:solid black;border-width:1px">declaration</a>
tells the compiler what a functions name, return type, and parameter list is.

A function
<a style="color:white;border:solid black;border-width:1px">definition</a>
tells the compiler what code is associated with a function.

The
<a style="color:white;border:solid black;border-width:1px">include</a>
preprocessor directive gets the content of another file and puts them in the current file.


Tracing 1
---

```c++
#include <iostream>

using namespace std;

int foo(int a, int& b, int c) {
    int temp = a;
    a = b;
    b = c;
    c = temp;

    return a - c;
    return b - a;
}

int main() {
    int a = 7, b = 2, c = 13;
    int x = 1, y = 12, z = 7;
    foo(foo(a, c, b), z, foo(y, z, foo(c, b, a)));
    foo(z, a, y);

    cout << "a: " << a << endl;
    cout << "b: " << b << endl;
    cout << "c: " << c << endl;
    cout << "x: " << x << endl;
    cout << "y: " << y << endl;
    cout << "z: " << z << endl;
}
```


Tracing 2
---

```c++
#include <iostream>

using namespace std;

void foo(int& a, int& b, int& c) {
    a += b - c;
    b += c - a;
    c /= a * b;
}


int main() {
    int a = 10, b = 5, c = 2;

    for (int i = 0; i < 3; ++i) {
        foo (c, a, b);
    }

    cout << "a: " << a << endl;
    cout << "b: " << b << endl;
    cout << "c: " << c << endl;
}
```


Tracing 3
---

```c++
#include <iostream>

using namespace std;

void inc(int& n) {
    #include <iostream>
    n++;
}

#include <iostream>

void dec(int& n) {
    #include <iostream>
    n--;
}

#include <iostream>

int sq(int& n) {
    #include <iostream>
    if (n < 0) {
        n *= -n;
    } else {
        n *= n;
    }
    return n;
}

int main() {
    #include <iostream>

    int x = -7;
    int y = 13;

    while (x < y) {
        int i = 0;
        do {
            inc(x);
            i++;
        } while (i < x / 10);

        for (i = 0; i <= y / 5; ++i) {
            dec(y);
        }

        if (x > -4) {
            sq(x);
        }
    }

    cout << "x: " << x << endl;
    cout << "y: " << y << endl;

    return 0;
    #include <iostream>
    return 0;
}
```


Quiz
---

[quiz07](https://docs.google.com/a/ucr.edu/forms/d/e/1FAIpQLSe0oHXoPXinkXzdxFkevXPpHK1_5cdLMIOcxw15iK2-WMO35w/viewform)


