# C Programming

<img src="https://contentstatic.techgig.com/photo/90325682.cms" alt="C Programming" height="350px" width="350px">

# Table of Content
* Introduction
* Introduction of C Programming
* Installation
* System Requirement


# Introduction of C Programming
* Programming- Computer programming is a medium for us to communicate with computers.Just like humans hindi/English to communicate which other,Programming is a way to deliver our instrutions to the computer.
* C is one of the oldest and finest Programming language which is developed by Dennis Ritchie in 1972.
* It was developed as a system programming language to write the UNIX operating system.
* C Programming is used to program embedded systems where programs need to run faster in limited memory.

# Features of C 
<img src="https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2021/08/Features-of-C.jpg" alt="Features" height="350px" width="350px">" 

  # Module 1- Variables, Constant & Keywords
  ## Variables
  * Variables in programming are used to store piece of information.
  * It's type of COntainers storing some data (for eg. we store rice,dal, sugar in different containers)
    ### Rules of naming Variables
    * The first character must be an alphabet or underscore(_).
      NOTE :- No special symbols rather than underscore is allowed.
    * NO commas or blanks are allowed.
    * Variables names are Case senstive. eg- int STUDENT=10; , int student=10; (Both STUDENT and student are different variable
    ### Syntax of declaring Variable
   <img src="https://media.geeksforgeeks.org/wp-content/uploads/20221202181339/Cvariables1.png" alt="Features" height="250px" width="550px">" 

   ### WAP for Variables
   ```
#include <stdio.h>

int main() {
    // Declaring variables of different types
    int age = 25;                // Integer variable
    float height = 5.9;          // Float variable
    char initial = 'A';          // Character variable
    double salary = 50000.75;    // Double variable
    char name[] = "Alice";       // String (array of characters)

    // Printing the values of the variables
    printf("Age: %d\n", age);               // %d is used for integers
    printf("Height: %.1f\n", height);       // %.1f is used for floats with one decimal place
    printf("Initial: %c\n", initial);       // %c is used for characters
    printf("Salary: %.2f\n", salary);       // %.2f is used for doubles with two decimal places
    printf("Name: %s\n", name);             // %s is used for strings
}
```
  ### Output
```
Age: 25
Height: 5.9
Initial: A
Salary: 50000.75
Name: Alice


=== Code Execution Successful ===
```

   

   
  





