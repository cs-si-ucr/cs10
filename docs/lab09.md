Instructions
---

READ EACH EXERCISE CAREFULLY!

Make sure you understand the problem before attempting to code the solution.
Please ask your SI Leader for clarification if you are having trouble understanding the problem.

Complete exercises 1 through 4, then write tests for all of them.
Show your tests to the SI leader.
You are allowed to use assert.


Exercise 1
---

Write a function that takes as input a vector, and prints to the terminal the contents of the vector.
This will be useful for testing the output of the rest of the exercises.

To do this you need to know how to define a vector, iterate through a vector, and how to access vector elements.

You can use the following code as a template for this exercise.

```c++
#include <iostream>

using namespace std;

// YOUR FUNCTION DECLARATION HERE

int main(){
    vector<int> myVec;
    for (int i = 1; i <= 6; ++i) {
        myVec.push_back(i);
    }
    print(myVec);
    return 0;
}

// YOUR FUNCTION DEFINITION HERE
```

The above code when completed should output something like: {1, 2, 3, 4, 5, 6}


Exercise 2
---

The first few numbers of the Fibonacci sequence are `0, 1, 1, 2, 3, 5, 8, 13, ...`

Each term in the Fibonacci sequence is defined as the sum of the previous two numbers in the sequence.
The first two numbers are 0 and 1 because those two sequence values each do not have two previous terms.

Write a function that accepts an integer `n` and returns a vector that contains the first `n` Fibonacci numbers.


Exercise 3
---

Write a function that reverses a vector of strings.
The function should accept a reference to a vector.
The function should not return anything. 

*Bonus*:
Modifiy your code to also reverse each string.


Exercise 4
---

Say I want to shoot myself out of a cannon;
I might as well go as far as possible!
<i>if I am going to do such a thing...</i>

I need to write a program that can help me estimate what angle I have to launch to go the furthest.

I wrote some of the program already, but since I am a lazy SI leader, I am going to have you write the rest.
Given the code below, fill out the sections labeled TODO to determine the correct launch angle.

Make sure you understand what the helper function `getDistance` is doing.
The details are not important, but knowing how to use it is.

Remember to ask questions if you are struggling!

```c++
#include <iostream>
#include <vector>
#include <cmath>

using namespace std;

double getDistance(double, double);
double metersToMiles(double);

int main() {
    const int min_angle = 20;    // The minimum angle
    const int max_angle = 70;    // The maximum angle
    const int angle_inc = 1;     // The amount I increment the angle
    const double velocity = 120; // My initial velocity as I leave the cannon
    vector<double> angles;       // Vector for storing angles
    vector<double> distances;    // Vector for storing distances 

    // TODO: Store the angles we will be using to calculate the distance 
   

    // TODO: Store the impact distance for each angle 


    // TODO: Find the maximum distance and corresponding angle


    // TODO: Output the result
    

    return 0;
}

// Returns the distance where I impact the ground given a velocity and angle
double getDistance(double velocity, double angle) {
    const double pi = 3.14;                          // constant for pi
    const double gravity = 9.81;                     // gravity constant for earth
    double radians = (angle * pi / 180);             // convert angle to radians
    double velocity_y = velocity * sin(radians);     // velocity in y direction
    double velocity_x = velocity * cos(radians);     // velocity in x direction
    double impact_time = (2 * velocity_y) / gravity; // the time when I hit the ground
    return metersToMiles(velocity_x * impact_time);  // the total distance I traveled
}

// Converts from meters to miles
double metersToMiles(double meters) {
    return meters / 1609.34;
}                       
```

*Bonus*:
Look up different gravity values, such as on the moon or Jupiter.
How far could I go on those planets?


