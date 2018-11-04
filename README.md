# iterations
C++ Module for Calculating Iterations


This module counts iterations in your code (function calls (recursions) , and while/for loops).
Warning! It doesn't currently work with file stream in/out (counts too many iterations)

Instalation:
1. Copy and link "iterations" file to your C++ project
2. Add compiler flag "-finstrument-functions" to your project
3. Include iterations module in your cpp file (#include "iterations")

Data Types:

tick_int (which is actually "unsigned long long int", but shortened version)


Functions:

tick_int get_ticks() - Gets number of iterations from the time program started (or function reset_ticks called)
tick_int reset_ticks() - Resets current iterations to 0.


Basically you would use them like this:



reset_counter() // setting our counter to value 0


// Your code here....

tick_int result = get_ticks();

// Now for example print result

cout << "Number of iterations of my code: " << result;



P.S. For more details see: example.cpp
