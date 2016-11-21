Introduction
---
An 
<a style="color:white;border:solid black;border-width:1px">array/vector</a>
is a special variable having one name, but storing a list of data items, with each item directly accessible.

Each item in an array/vector is known as an 
<a style="color:white;border:solid black;border-width:1px">element</a>
.

In an array/vector, each element's location number is called the 
<a style="color:white;border:solid black;border-width:1px">index</a>
.

<a style="color:white;border:solid black;border-width:1px">Arrays</a>
are native to c++ while
<a style="color:white;border:solid black;border-width:1px">vectors</a>
are not.

<a style="color:white;border:solid black;border-width:1px">vctr.push_back(value)</a>
creates a new element at the end of the vector and assigns the given value to that element.

A vector's size can be set or changed while a program is executing using 
<a style="color:white;border:solid black;border-width:1px">vctr.resize(N)</a>
.

<a style="color:white;border:solid black;border-width:1px">Vectors</a>
are safer because the access b.at(i) is checked during execution to ensure the index is within the range. 
<a style="color:white;border:solid black;border-width:1px">Array's</a>
access b\[i\] involves no such check. 

<a style="color:white;border:solid black;border-width:1px">Vectors</a>
have more advantages than 
<a style="color:white;border:solid black;border-width:1px">arrays,</a>
like resizing during runtime, easy insertion of items at the front or rear, determining vector size, etc.

Tracing 1
---

```c++

```


Tracing 2
---

```c++
#include <iostream> 
#include <vector>

using namespace std;

//Prints the elements of vector v with spaces separating each element
void printVector(vector<int> v){
    for(int i = 0; i < v.size(); i++){
        if(i < v.size() - 1){
            cout << v.at(i) << ' ';
        }
        else{
            cout << v.at(i);
        }
    }
}

int main(){
    vector<int> v;
    
    for (int i = 5; i > 0; i--){
        v.push_back(i);
    }
    
    printVector(v);
    cout << endl;
    
    for (int i = 0; i < v.size() - 1; i++){
        for (int j = 0; j < v.size() - i - 1; j++){
           if (v.at(j) > v.at(j + 1)){
              swap(v.at(j), v.at(j + 1));
           }
        }
    }
    
    printVector(v);
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

//Prints the elements of vector v with spaces separating each element
void printVector(vector<int> v){
    for(int i = 0; i < v.size(); i++){
        if(i < v.size() - 1){
            cout << v.at(i) << ' ';
        }
        else{
            cout << v.at(i);
        }
    }
}

int main(){
    /*The following code sets up the 2d vectors:
    
       a:  5 3    and   b:  1 3
           4 2              2 4
    */
    vector<vector<int> > a;
    vector<vector<int> > b;
    vector<vector<int> > r;
    vector<int> ac1(2);
    vector<int> ac2(2);
    vector<int> bc1(2);
    vector<int> bc2(2);
    vector<int> rc1(2);
    vector<int> rc2(2);
    
    ac1.at(0) = 5;
    ac1.at(1) = 3;
    ac2.at(0) = 4;
    ac2.at(1) = 2;
    
    bc1.at(0) = 1;
    bc1.at(1) = 3;
    bc2.at(0) = 2;
    bc2.at(1) = 4;
    
    rc1.at(0) = 0;
    rc1.at(1) = 0;
    rc2.at(0) = 0;
    rc2.at(1) = 0;
    
    a.push_back(ac1);
    a.push_back(ac2);
    
    b.push_back(bc1);
    b.push_back(bc2);
    
    r.push_back(rc1);
    r.push_back(rc2);
    
    //Print the two 2d vectors a and b
    printVector(a.at(0));
    cout << endl;
    printVector(a.at(1));
    cout << endl;
    cout << endl;
    printVector(b.at(0));
    cout << endl;
    printVector(b.at(1));
    cout << endl;

    //START TRACING HERE
    for(int i = 0; i < a.at(0).size(); i++){
        for(int j = 0; j < a.size(); j++){
            for(int k = 0; k < b.size(); k++){
                r.at(i).at(k) += a.at(i).at(j) * b.at(j).at(k);
            }
        }
    }
    
    //Print the two 2d vector r
    cout << endl;
    printVector(r.at(0));
    cout << endl;
    printVector(r.at(1));
    cout << endl;
    
    return 0;
}
```


Quiz
---

[Quiz]()


