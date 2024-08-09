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
 ### These are Arithmetic Operators : 
   ```
     S. No.	 Symbol	   Operator	             Description             	                  Syntax
        1	    +         Plus	       Adds two numeric values.	                            a + b
        2	    –	        Minus	      Subtracts right operand from left operand.         	 a – b
        3	    *	        Multiply   	Multiply two numeric values.                      	  a * b
        4	    /      	  Divide     	Divide two numeric values.	                          a / b
        5	    %        	Modulus    	Returns the remainder after diving the left         	a % b
                                   operand with the right operand.
   ```
  
   *Program for Arithmetic Operator
   ```
   #include <stdio.h>
    int main() {
    int num1,num2;
     printf("Enter first number: ");
    scanf("%d", &num1);
     printf("Enter Second number: ");
    scanf("%d", &num2);
    printf("num1+num2 = %d\n ", num1+num2);
    printf("num1-num2 = %d\n ", num1-num2);
    printf("num1*num2 = %d\n ", num1*num2);
    printf("num1/num2 = %d\n ", num1/num2);
   printf("num1%num2 = %d\n ", num1%num2);
    return 0;
}
```

### Output
```
Enter first number: 7
Enter Second number: 9
 num1+num2 = 16
 num1-num2 = -2
 num1*num2 = 63
 num1/num2 = 0
 num1%num2 = 1
=== Code Execution Successful ===
```
## Relational Operators 
* The relational operators in C are used for the comparison of the two operands.
* All these operators are binary operators that return true or false values as the result of comparison.

### These are Relational Operators
```
S. No.	  Symbol	     Operator	                              Description	                                                                  Syntax
1	         <	         Less than	                  Returns true if the left operand is less than the right operand. Else false	             a < b
2         	>	         Greater than       	        Returns true if the left operand is greater than the right operand. Else false	          a > b
3	        <=	         Less than or equal to      	Returns true if the left operand is less than or equal to the right operand. Else false	 a <= b
4	        >=	         Greater than or equal to	   Returns true if the left operand is greater than or equal to right operand. Else false	  a >= b
5     	   ==	         Equal to	                   Returns true if both the operands are equal.	                                            a == b
6	        !=	          Not equal to	              Returns true if both the operands are NOT equal.                                        	a != b
```
 ### Program for Relational Operators
```
#include <stdio.h>
int main() {
    int a, b;
    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    //  Relational operators
    printf("%d == %d is %d\n", a, b, a == b);   // Equal to
    printf("%d != %d is %d\n", a, b, a != b);   // Not equal to
    printf("%d > %d is %d\n", a, b, a > b);     // Greater than
    printf("%d < %d is %d\n", a, b, a < b);     // Less than
    printf("%d >= %d is %d\n", a, b, a >= b);   // Greater than or equal to
    printf("%d <= %d is %d\n", a, b, a <= b);   // Less than or equal to
    return 0;
}
```

### Output

```
Enter two integers: 10 20
10 == 20 is 0
10 != 20 is 1
10 > 20 is 0
10 < 20 is 1
10 >= 20 is 0
10 <= 20 is 1
=== Code Execution Successful ===
```

## Logical Operator
* The logical operators in c help a user determine if the results would be true or false.
* These are Logical Operators:
  
```
S.No.	Symbol	  Operator	     Description	                                          Syntax
1	     &&	     Logical AND	  Returns true if both the operands are true.	          a && b
2	     ||	     Logical OR	   Returns true if both or any of the operand is true.	  a || b
3	     !	      Logical NOT	  Returns true if the operand is false.	                 !a
```

### Program for Logical Operators
```
#include <stdio.h>
int main() {
    int a, b;
    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    //Logical AND (&&)
    if (a > 0 && b > 0) {
        printf("Both a and b are positive.\n");
    } else {
        printf("Either a or b (or both) are not positive.\n");
    }

    // Logical OR (||)
    if (a > 0 || b > 0) {
        printf("At least one of a or b is positive.\n");
    } else {
        printf("Neither a nor b is positive.\n");
    }

    // Logical NOT (!)
    if (!(a > 0)) {
        printf("a is not positive.\n");
    } else {
        printf("a is positive.\n");
    }

    return 0;
}
```
### Output
```
Enter two integers: 10 -10
Either a or b (or both) are not positive.
At least one of a or b is positive.
a is positive.

=== Code Execution Successful ===
```
## Bitwise Operators
* The Bitwise operators are used to perform bit-level operations on the operands.
* Mathematical operations such as addition, subtraction, multiplication, etc. can be performed at the bit level for faster processing.
* These are Bitwise Operators
  ```
    S.No.	  Symbol	  Operator	                Description	                                                                                  Syntax
     1	       &	     Bitwise AND	             Performs bit-by-bit AND operation and returns the result.	                                     a & b
     2	       |	     Bitwise OR	              Performs bit-by-bit OR operation and returns the result.                                      	a | b
     3	       ^	     Bitwise XOR	             Performs bit-by-bit XOR operation and returns the result.                                      	a ^ b
     4	       ~	     Bitwise First Complement	Flips all the set and unset bits on the number.	                                                 ~a
     5	      <<     	Bitwise Leftshift	       Shifts the number in binary form by one place in the operation and returns the result.         	a << b
     6	      >>     	Bitwise Rightshilft	     Shifts the number in binary form by one place in the operation and returns the result.	         a >> b

``

### Program for Bitwise Operators

```
#include <stdio.h>
int main() {
    int a, b;
    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Bitwise AND
    printf("%d & %d = %d\n", a, b, a & b);

    // Bitwise OR
    printf("%d | %d = %d\n", a, b, a | b);

    // Bitwise XOR
    printf("%d ^ %d = %d\n", a, b, a ^ b);

    // Bitwise NOT (only for 'a' as an example)
    printf("~%d = %d\n", a, ~a);

    // Left Shift (shifting 'a' by 1)
    printf("%d << 1 = %d\n", a, a << 1);

    // Right Shift (shifting 'a' by 1)
    printf("%d >> 1 = %d\n", a, a >> 1);

    return 0;
}
```


### Output
```
Enter two integers: 5 3
5 & 3 = 1
5 | 3 = 7
5 ^ 3 = 6
~5 = -6
5 << 1 = 10
5 >> 1 = 2

=== Code Execution Successful ===
```
## Assignment Operators
* Assignment operators are used to assign value to a variable.
* These are Assignment Operators :
  ```
  S. No.  	Symbol	     Operator	                                 Description	                                                                   Syntax
    1	      =	       Simple Assignment	      Assign the value of the right operand to the left operand.	                                         a = b
    2	      +=	      Plus and assign	       Add the right operand and left operand and assign this value to the left operand.	                   a += b
    3	      -=	      Minus and assign      	Subtract the right operand and left operand and assign this value to the left operand.	              a -= b
    4      	*=	     Multiply and assign	    Multiply the right operand and left operand and assign this value to the left operand.	              a *= b
    5      	/=	      Divide and assign	     Divide the left operand with the right operand and assign this value to the left operand.	           a /= b
    6      	%=	     Modulus and assign	    Assign the remainder in the division of left operand with the right operand to the left operand.     	a %= b
    7	      &=	     AND and assign	        Performs bitwise AND and assigns this value to the left operand.	                                     a &= b
    8	      |=	     OR and assign          Performs bitwise OR and assigns this value to the left operand.	                                      a |= b
   9	       ^=	     XOR and assign	        Performs bitwise XOR and assigns this value to the left operand.                                      	a ^= b
   10      	>>=	    Rightshift and assign	 Performs bitwise Rightshift and assign this value to the left operand.                               	a >>= b
   11      	<<=	    Leftshift and assign	  Performs bitwise Leftshift and assign this value to the left operand.	                                a <<= b
				```
### Example of Assignment Operators
```
#include <stdio.h>
int main(){
    int a = 25, b = 5;
    //  Assignment Operators
    printf("a = b: %d\n", a = b);
    printf("a += b: %d\n", a += b);
    printf("a -= b: %d\n", a -= b);
    printf("a *= b: %d\n", a *= b);
    printf("a /= b: %d\n", a /= b);
    printf("a %%= b: %d\n", a %= b);
    printf("a &= b: %d\n", a &= b);
    printf("a |= b: %d\n", a |= b);
    printf("a >>= b: %d\n", a >>= b); 
    printf("a <<= b: %d\n", a <<= b);

    return 0;
}
```
### Output
```
a = b: 5
a += b: 10
a -= b: 5
a *= b: 25
a /= b: 5
a %= b: 0
a &= b: 0
a |= b: 5
a >>= b: 0
a <<= b: 0
```
## Unary Operators 
* Unary operators are the operators that perform operations on a single operand to produce a new value.
  ### Types of Unary Operators
  #### Unary Plus (+) Operator
* The unary plus operator doesn't affect the value of its operand. However, it can improve code readability and indicate the positive value.
  ```
  int x = +5;
printf("%d\n", x);  // Output: 5
``
#### Unary Minus (-) Operator
* The unary minus operator negates the value of its operand. If it's applied to a positive value, the value becomes negative, and vice versa.
  ```
  int x = -5;
printf("%d\n", x);  // Output: -5
``
#### Increment (++) Operator
* This unary operator in C increases the value of its operand by 1.
 ```
  int x = 5;
x++;
printf("%d\n", x);  // Output: 6
```
#### Decrement (--) Operator
* The decrement operator decreases the value of its operand by 1.
  ```
int x = 5;
x--;
printf("%d\n", x);  // Output: 4
``
#### Address of (&) Operator in C
* This operator returns the memory address of its operand.
```
int x = 5;
printf("%p\n", &x);  // Output: Memory address of x
```
#### Sizeof() Operator
* The sizeof operator returns the size (in bytes) of its operand.
 ```
int x;
printf("%zu\n", sizeof(x));  // Output: Size of integer on your system, commonly 4
```

## Conditional/ Ternary Operator
* Ternary operator is the shorthand way or writing an if-else statement.
### Syntax 
```
Cndition? expression-if-true: expression-if-false;
```
### Example 
```
#include<stdio.h>
int main(){
    int a;
    printf("Enter value of a\n");
    scanf("%d",&a);
    (a<5)?printf("A is less than 5"):printf("A is not less than 5");
    return 0;
}
```
### Output
```
Enter value of a
7
A is not less than 5ements

=== Code Execution Successful ===
```
# Module 3 - Control Statements Decision-Making
* COntrol statements are the statements which are used to control the flow of execution of the instructions.
    <img src="https://examradar.com/wp-content/uploads/2016/10/Classification-of-control-statements.png" alt="Control statements" width="450px" height="350px">
    ## Branching Statements
  ### If Statements
  * "if" statement is a control flow structure that allows you to execute a block of code conditionally, based on whether a specified condition is true or false.
   ##### Example
  ```
  #include <stdio.h>
  int main() {
    int number = 10;
    if (number > 5) {
        printf("The number is greater than 5.\n");
     }
  }
  ```
  #### Output
  ```
  The number is greater than 5.
  ```
  ### If-else Statements
  * The if-else statement in C is a conditional control structure that allows you to execute one block of code if a condition is true, and another block of code if the condition is false.
    #### Example
    ```
    #include <stdio.h>
    int main() {
    int number = 3;
    if (number > 5) {
        printf("The number is greater than 5.\n");
    } else {
        printf("The number is 5 or less.\n");
      }
  }
  ``
  #### Output
  ```
  The number is 5 or less.
  ```
  ### If-else-if Statements
  * The if-else if statement in C is used to test multiple conditions in sequence.
  * It allows you to execute different blocks of code depending on which condition is true.
    #### Example
    ```
    #include <stdio.h>  
    int main() {
    int number = 0;
    if (number > 0) {
        printf("The number is positive.\n");
    } else if (number < 0) {
        printf("The number is negative.\n");
    } else {
        printf("The number is zero.\n");
    }
 }
``
#### Output
```
The number is zero.
```
### Switch Statements
* The switch statement in C is a control flow structure that allows the execution of different code blocks based on the value of an expression.
#### Exaample
```
#include <stdio.h>
int main() {
    int day = 3;
    switch (day) {
        case 1:
            printf("Monday\n");
            break;
        case 2:
            printf("Tuesday\n");
            break;
        case 3:
            printf("Wednesday\n");
            break;
        case 4:
            printf("Thursday\n");
            break;
        case 5:
            printf("Friday\n");
            break;
        case 6:
            printf("Saturday\n");
            break;
        case 7:
            printf("Sunday\n");
            break;
        default:
            printf("Invalid day\n");
            break;
    }
}
```
#### Output
```
Wednesday
```
## Iterative/ Loop Statements 
* Iterative or loop statements are used to execute a block of code repeatedly based on a condition.
*  They allow for performing repetitive tasks efficiently without needing to write the same code multiple times.
   ### For Loop
   * Loop statements are used to execute the set of instructions in a repeated order.
   *  The execution of the set of instructions depends upon a particular condition.
   *  #### Example
    ```
    #include <stdio.h>
     int main() {
    // Loop from 0 to 4
    for (int i = 0; i < 5; i++) {
        printf("Number %d\n", i);
    }
}
``
### Output
```
Number 0
Number 1
Number 2
Number 3
Number 4
```
### While Loop
* The while loop in C is a control flow statement that allows you to execute a block of code repeatedly as long as a specified condition is true
