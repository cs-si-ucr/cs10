Introduction
---

A 
<a style="color:white;border:solid black;border-width:1px">vector</a>
is a special type that is used to create variables with a single name and multiple data items.

Each item in an array/vector is known as an 
<a style="color:white;border:solid black;border-width:1px">element</a>.

In a vector, each element location number is called an
<a style="color:white;border:solid black;border-width:1px">index</a>.

<a style="color:white;border:solid black;border-width:1px">Arrays</a>
are native to c++ while
<a style="color:white;border:solid black;border-width:1px">vectors</a>
are not.
They perform similarly, however.

The
<a style="color:white;border:solid black;border-width:1px">push_back</a>
member function creates a new element at the end of the vector and assigns its argument to that element.

The size of a vector can be set to a specific value using the
<a style="color:white;border:solid black;border-width:1px">resize</a>
member function.

Vectors are safer to use than arrays because the
<a style="color:white;border:solid black;border-width:1px">at</a>
member function checks if an element exists before accessing it.

<a style="color:white;border:solid black;border-width:1px">Vectors</a>
are easier to use than 
<a style="color:white;border:solid black;border-width:1px">arrays</a>
because of the ability to determine size, resize, and insert and remove items at the rear.


Tracing 1
---

```c++
#include <iostream> 
#include <vector>

using namespace std;

int main() {
    vector<int> a;
    vector<int> b;
    int r = 0;
    
    a.push_back(3);
    a.push_back(5);
    a.push_back(1);
    
    b.push_back(-2);
    b.push_back(4);
    b.push_back(6);
    
    // Bonus: what operation is being performed here?
    for (int i = 0; i < a.size(); i++) {
        r += a.at(i) * b.at(i);
    }
    
    cout << r << endl;
    
    return 0;
}
```

Tracing 2
---

```c++
#include <iostream> 
#include <vector>

using namespace std;

// Prints the elements of vector v vertically
void printVerticalVector(const vector<int> &v) {
    for (int i = 0; i < v.size(); i++) {
        if (i < v.size() - 1) {
            cout << v.at(i) << endl;
        }
        else {
            cout << v.at(i);
        }
    }
}

int main() {
    vector<int> a;
    vector<int> b;
    vector<int> r;
    
    a.push_back(3);
    a.push_back(5);
    a.push_back(1);
    
    b.push_back(2);
    b.push_back(4);
    b.push_back(6);
    
    // Bonus: what operation is being performed here?
    r.push_back(a.at(1) * b.at(2) - a.at(2) * b.at(1));
    r.push_back(a.at(2) * b.at(0) - a.at(0) * b.at(2));
    r.push_back(a.at(0) * b.at(1) - a.at(1) * b.at(0));
    
    printVerticalVector(r);
    cout << endl;
    
    return 0;
}
```

Tracing 3
---

```c++
#include <iostream> 
#include <vector>

using namespace std;

// Prints the elements of vector v with spaces separating each element
void printVector(const vector<int> &v) {
    if (v.size() == 0) return;
    for (int i = 0; i < v.size() - 1; i++) {
        cout << v.at(i) << ' ';
    }
    cout << v.at(v.size() - 1);
}

int main(){
    vector<int> v;
    
    v.push_back(3);
    v.push_back(2);
    v.push_back(-1);
    v.push_back(1);
    v.push_back(4);
    
    printVector(v);
    cout << endl;
    
    for (int i = 0; i < v.size() - 1; i++) {
        for (int j = 0; j < v.size() - i - 1; j++) {
           if (v.at(j) > v.at(j + 1)) {
              swap(v.at(j), v.at(j + 1));
           }
        }
    }
    
    printVector(v);
    cout << endl;
    
    return 0;
}
```


Tracing 4
---

```c++
#include <iostream> 
#include <vector>

using namespace std;

// Prints the elements of vector v with spaces separating each element
void printVector(const vector<int> &v) {
    if (v.size() == 0) return;
    for (int i = 0; i < v.size() - 1; i++) {
        cout << v.at(i) << ' ';
    }
    cout << v.at(v.size() - 1);
}

int main() {
    vector<vector<int> > a;
    vector<vector<int> > b;
    vector<vector<int> > r;
    vector<int> ar1(2);
    vector<int> ar2(2);
    vector<int> br1(2);
    vector<int> br2(2);
    vector<int> rr1(2);
    vector<int> rr2(2);
    
    ar1.at(0) = 5;
    ar1.at(1) = 3;
    ar2.at(0) = 4;
    ar2.at(1) = 2;
    
    br1.at(0) = 1;
    br1.at(1) = 3;
    br2.at(0) = 2;
    br2.at(1) = 4;
    
    rr1.at(0) = 0;
    rr1.at(1) = 0;
    rr2.at(0) = 0;
    rr2.at(1) = 0;
    
    a.push_back(ar1);
    a.push_back(ar2);
    
    b.push_back(br1);
    b.push_back(br2);
    
    r.push_back(rr1);
    r.push_back(rr2);

    for (int i = 0; i < a.at(0).size(); i++) {
        for (int j = 0; j < a.size(); j++) {
            for (int k = 0; k < b.size(); k++) {
                r.at(i).at(k) += a.at(i).at(j) * b.at(j).at(k);
            }
        }
    }
    
    printVector(r.at(0));
    cout << endl;
    printVector(r.at(1));
    cout << endl;
    
    return 0;
}
```

Tracing 5
---

```c++
#include <iostream>
#include <vector>
using namespace std;

// Prints the elements of vector v with spaces separating each element
void printVector(const vector<int> &v) {
    if (v.size() == 0) return;
    for (int i = 0; i < v.size() - 1; i++) {
        cout << v.at(i) << ' ';
    }
    cout << v.at(v.size() - 1);
}

int mod(vector<int> &a, int sz) {
    for(int x=0; x <= sz; x += 2) {
        swap(a.at(x), a.at(x%3));
    }
    return a.at(sz % 3) % 3;
}
 
void check(int &c, int sz) {
    // cout << c << '\t' << sz << '\t' << (int)(c-'a') << endl;
    if(sz >= c - sz) {
        c++;
    } else {
        c--;
    }
}

int main() {
    ///////////////////////////////////// 1 ////////////////////////////////////
    vector<int> a = {1, 2, 3, 4, 5};
    check(a.at(0), mod(a, 5));
    printVector(a);
    cout << endl;
   
    ///////////////////////////////////// 2 ////////////////////////////////////
    // The next line sets boolean value printing to display "false" or "true" instead of 0 or 1
    cout << boolalpha;
    vector<int> b = {3, 19, 18, 21, 12, 5, 19};
    vector<int> c = {4, 15, 23, 14, 23, 9, 20, 8, 5, 5};
    // Comparing vectors looks at each value until it finds two that are diff
    //     if the element on the left is less than the element on the right, the expression evaluates to true
    //     otherwise, it evaluates to false.
    cout << (b < c) << endl; // will output true because b.at(0) < c.at(0)
    cout << mod(b, 6) << endl;
    cout << (b < c) << endl;
   
    ///////////////////////////////////// 3 ////////////////////////////////////
    printVector(b);
    cout << endl;
    for(int x=0; x < b.size(); x++) {
        check(b.at(x), x);
    }
    printVector(b);
    cout << endl;
   
    return 0;
}
```
