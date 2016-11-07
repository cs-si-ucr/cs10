Introduction
---
A <a style="color:white;border:solid black;border-width:1px">function</a>
is a named block of code. Invoking a function name, knows as a
<a stlye="color:white;border:solid black;border-width:1px">function call</a>
causes the functions statements to execute.

A function
<a style="color:white;border:solid black;border-width:1px">definition</a>
consists of a new functions name and is sometimes followed by the preceding block of statements. 

In the statement
```c++
void Print(string strName)	
```
strName is a
<a style="color:white;border:solid black;border-width:1px">parameter</a>.
A function may have multiple parameters, seperated by
<a style="color:white;border:solid black;border-width:1px">commas</a>.
A function definiton without parameters must still have parenthasis. 
The value passed to a parameter is kmown as an <a style="color:white;border:solid black;border-width:1px">agrument</a>.

Each function must have a
<a style="color:white;border:solid black;border-width:1px">return</a>
statement which tranfers control of the program back to the where the functions was originally called.

The value of the return statement depends on how the function is defined. For
 example, in the function ``int main()`` a function named main is declared to
 have a type of 
<a style="color:white;border:solid black;border-width:1px">int</a>.
If a function is declared to be ``void`` as it is in the example above, then
 the return statement should simply be 
<a style="color:white;border:solid black;border-width:1px">return;</a>

Designating blocks of codes as functions can be useful for three reasons:</br>
>1) Improving program
<a style="color:white;border:solid black;border-width:1px">readability</a></br>
>2) <a style="color:white;border:solid black;border-width:1px">Modular</a>
program development </br>
>3) Avoiding
<a style="color:white;border:solid black;border-width:1px">redundant</a>
code


Code Tracing
---

What do the following programs output?

1)
```c++
void foo(int a, int b){
	a += 6;
	b += a;
	b = a * b;
	a = a + b;
	cout << a << endl;
	cout << b << endl;
}

int main(){
	int a = 5;
	int b = 3;
	cout << "Functions" << endl;
	foo(a,b);
	cout << "take parameters." << endl;

	return 0;
}
```
2)
```c++
void print(){
	cout << "the bomb" << endl;
}
void printb(){
	cout << "dot com" << endl;
}

void foo(int a){
	if(a < 5){
		printa();
	}
	else if(a == 5){
		printb();
	}
	else{
		cout << "none" << endl;
	}
}

int main(){
	int a = 5;
	int b = -5;
	foo(a);
	foo(b);

	return 0;
}
```
3)
```c++
int foo2(int b){
	int c = b + 6;
	if(c > 13){
		b = b + 5;
	}
	else{
		b = b + 9;
	}
	
	return c + b;
}

int foo(int a){
	if(a > -1){
		return -1;
	}
	else if(a < 0){
		return 0;
	}
}

int main(){
	int a = 0;
	int b = 7;
	if(foo(a) == 1){
		cout << "Positive!" << endl;
	}
	else{
		cout << "Negative!" << endl;
	}

	cout << foo2(b) + foo(a) << endl;

	return 0;
}
```
[Mock Midterm](https://docs.google.com/a/ucr.edu/document/d/1DWX5sqdetz-Vz8RpabkYFdxSUa_Q3DhBsVA2ugZxeCQ/edit?usp=sharing)
