Introduction
------------


Code Tracing
------------

What do the following programs output 
(If they dont compile what is wrong with the program?) :


```c++
// 1
using namespace std;

int main(){
   cout << "Hello World!"

   return 0;
}

// 2
#include <iostream>
using namespace std;

int main(){
   cout << "Does"; 
   cout << This;
   cout << ""Print"";
   cout << ?;

   return 0;
}

// 3
#include <iostream>
using namespace std;

int main(){
   cout << "How ";
   cout << "About";
   cout << " \"This\";
   cout << "?";
   cout << endl;

   return 0;
}

//4
#include <iostream>
using namespace std;

int main(){
   int test = 1;
   string temp = "line";
   // The above two lines are variable declarations
   // we will focus on this more next week
   /* Tip:
   * multi-line comments can also be written like this!
     FYI. */

   cout << "Let's just write everything on" << test << temp << endl;

   return 0;
}

```

* For future reference, we will assume that the lines:

```c++
#include <iostream>
using namespace std;
```
are included at the top of the program, even if not shown.

