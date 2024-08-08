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
<img src="https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2021/08/Features-of-C.jpg" alt="Features" height="350px" width="350px">

 # Comments in C
 In C there are two types of comments in C language:
* Single-line comment
* Multi-line comment
  
  ### Single-line Comment
A single-line comment in C starts with ( // ) double forward slash. It extends till the end of the line and we don’t need to specify its end.
```
// This is a single line comment
```
 ###  Multi-line comment
* The Multi-line comment in C starts with a forward slash and asterisk ( /* ) and ends with an asterisk and forward slash ( */ ). Any text between /* and */ is treated as a comment and is ignored by the compiler.
* It can apply comments to multiple lines in the program.
```
/* Hello Isha
Are You Fine? */
```
# First Program in C
```
#include<stdio.h>
int main(){
   printf("Hello World");
   return 0;
}
```
### Output
```
Hello World
```

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
   <img src="https://media.geeksforgeeks.org/wp-content/uploads/20221202181339/Cvariables1.png" alt="Features" height="250px" width="550px">

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
## Constant
* The constants in C are the read-only variables whose values cannot be modified once they are declared in the C program.
* The type of constant can be an integer constant, a floating pointer constant, a string constant, or a character constant.
*  In C language, the const keyword is used to define the constants.
  ### Syntax of declaring Constant
  ```
const data_type var_name = value;
```
 <img src="https://media.geeksforgeeks.org/wp-content/uploads/20230306215927/syntax-of-constants-in-c.png" alt="Features" height="250px" width="550px">" 
 ### WAP of Constant
 ```
#include <stdio.h>

int main() {
    // Declare and initialize constant variables using the const keyword
    const int DAYS_IN_WEEK = 7;
    const int MONTHS_IN_YEAR = 12;
    const char GRADE = 'A';

    // Print the values of the constants
    printf("Number of days in a week: %d\n", DAYS_IN_WEEK);
    printf("Number of months in a year: %d\n", MONTHS_IN_YEAR);
    printf("Highest grade: %c\n", GRADE);

    // Attempting to modify the constants will result in a compile-time error
    // Uncommenting the following lines will cause errors
    // MONTHS_IN_YEAR = 10;
    // DAYS_IN_WEEK = 8;

    return 0;
}
```
### Output
```
Number of days in a week: 7
Number of months in a year: 12
Highest grade: A


=== Code Execution Successful ===
```
## Keywords
* Keywords in C refer to a set of reserved words with predefined meanings that are used to write programs in the C programming language.
* These keywords cannot be used as identifiers or variable names, as they have a specific function within the language.
  
 <img src="https://techskillguru.com/cdata/cprogramming/images/C-Keywords.png" alt="Features" height="350px" width="350px">

 # Module 2- Operators
 * In Programming, operators are symbols that represent operations to be performed on one or more operands.
 * An operator is defined as the symbol that helps us to perform some specific mathematical, relational, bitwise, conditional, or logical computations on values and variables.
    
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231214120748/Operators-in-C.png" alt="Features" height="350px" width="350px">" 

 ## Arithmetic Operators:
 * The arithmetic operators are used to perform arithmetic/mathematical operations on operands.
 * 
   
   ```
   #include <stdio.h>
    int main() {
    int num1,num2;
     printf("Enter first number: \n");
    scanf("%d", &num1);
     printf("Enter Second number: \n");
    scanf("%d", &num2);
    printf("num1+num2 = %d\n ", num1+num2);
    printf("num1-num2 = %d\n ", num1-num2);
    printf("num1*num2 = %d\n ", num1*num2);
    printf("num1/num2 = %d\n ", num1/num2);
   printf("num1%num2 = %d\n ", num1%num2);
    return 0;
}```

### Output
```
Enter first number: 
7
Enter Second number: 
9
 num1+num2 = 16
 num1-num2 = -2
 num1*num2 = 63
 num1/num2 = 0
 num1%num2 = 1
 
=== Code Execution Successful ===
```
## Relational Operators 
* The relational operators in C are used for the comparison of the two operands.

 ```
###  S. No.	 Symbol	  Operator	    Description             	                        Syntax
        1	    +       Plus	      Adds two numeric values.	                           a + b
        2	    –	      Minus	     Subtracts right operand from left operand.         	a – b
        3	    *	      Multiply  	Multiply two numeric values.                       	a * b
        4	    /      	Divide    	Divide two numeric values.	                         a / b
        5	    %      	Modulus   	Returns the remainder after diving the left        	a % b
                                   operand with the right operand.
```



   

   
  





