# C Programming

<img src="https://contentstatic.techgig.com/photo/90325682.cms" alt="C Programming" height="350px" width="450px">

# Table of Content
- [Introduction](#Introduction)
- [Installation](#Installation)
- [System Requirement](#System-Requirement)
- [Variables, Constant and Keywords](#Variables,-Constant-and-Keywords)
- [Operators](#Operators) 
- [Control Statements & Decision Making](#Control-Statements-&-Decision-Making)
- [Pointer](#Pointer)
- [Array](#Array)
- [String](#String)

# Introduction 
* Programming- Computer programming is a medium for us to communicate with computers. Just like humans uses hindi/English language to communicate which each other, Programming is the way to deliver our instructions to the computer.
* C is one of the oldest Programming language which is developed by Dennis Ritchie in 1972.

# Features 
<img src="https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2021/08/Features-of-C.jpg" alt="Features" height="350px" width="350px">

 # Comments in C
 In C there are two types of comments in C language:
* Single-line comment
* Multi-line comment
  
  ### Single-line Comment
 A single-line comment in C starts with ( // ) double forward slash. It extends until the end of the line and we don’t need to specify its end.
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
# Installation

To download Visual Studio Code ,you require to go through with the following steps:
* Step 1:- Search on browser to Download VsCode. 
* Step 2:- click on the first link.<a href="https://code.visualstudio.com/download">Visual Studio Code</a>
* Step 3:- Select the appropriate download as per your Operating System, If you are on a Ubuntu: your download will be a .deb file.
<img src="https://res.cloudinary.com/omaha-code/w_768,h_502,c_fit/omaha-code-cdn/2018/12/Download-Visual-Studio-Code.png" alt="VS Code" height="350px" width="450px">

* Step 4:- After download completion of VS Code,Open Terminal in Linux or for shortcut click (ctrl + alt + t).
* Step 5:- Check if the system up-to-date using following command :
```$ sudo apt update```
* Step 7:- After update system, Navigate to the Download Directory:
```cd ~/Downloads ```  
* Step 8:- Install the .deb Package by this command and enter your password:
  ```sudo dpkg -i code*.deb```
* Step 9:- Fix Dependencies:
    ```sudo apt install -f ```
* Step 10:-Launch VS Code:- You can now launch VS Code from the terminal by typing code, or find it in your application menu.         

   ![1](https://github.com/Amitkumar0054/HTML/assets/128821680/f181bcca-9f45-47e6-beda-5356498ac1b9)


# System Requirement
To use Visual Studio Code (VS Code) you need to ensure your system meets the following requirements for both VS Code.
* OS: Ubuntu 14.04+, Fedora 24+, CentOS 7+
* RAM: At least 4 GB of RAM (8 GB or more recommended)
* Disk Space: 512 MB of free disk space (2 GB or more recommended)
* Processor: pentium or faster processor

  My system configurations and software's versions:
* OS: Ubuntu 24.04 LTS
* RAM: 8GB
* Disk Space: 256 GB
* Processor: 11th Gen Intel Core i3
* VS Code Version: 1.91.1

  # Variables, Constant and Keywords
  ## Variables
  * Variables in programming are used to store pieces of information.
  * It's type of Containers storing some data (for eg. we store rice, dal, sugar in different containers).
    ### Rules of naming Variables
    * The first character must be an alphabet or underscore(_).
      NOTE :- No special symbols rather than underscore is allowed.
    * NO commas or blanks are allowed.
    * Variable names are Case sensitive. eg- int STUDENT=10; , int student=10; (Both STUDENT and student are different variable)
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
  Name: Alice``
 
## Constant
* The constants in C are the read-only variables whose values cannot be modified once they are declared in the program.
* The type of constant can be an integer constant, a floating pointer constant, a string constant, or a character constant.
* In C language, the const keyword is used to define the constant.
  ### Syntax of declaring Constant
  
 ```
 const data_type var_name = value;
 ```
 <img src="https://media.geeksforgeeks.org/wp-content/uploads/20230306215927/syntax-of-constants-in-c.png" alt="Features" height="250px" width="550px">
 
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
* Keywords in C refer to a set of reserved words with predefined meanings that are used to write programs in the C programming.
* These keywords cannot be used as identifiers or variable names, as they have a specific function within the language.
  
 <img src="https://techskillguru.com/cdata/cprogramming/images/C-Keywords.png" alt="Features" height="350px" width="350px">

 # Operators
 * In Programming, operators are symbols that represent operations to be performed on one or more operands.
   
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231214120748/Operators-in-C.png" alt="Features" height="350px" width="350px">" 

 ## Arithmetic Operators:
 * The arithmetic operators are used to perform arithmetic/mathematical operations on operands.
 ### These are Arithmetic Operators :
 
| S. No. | Symbol | Operator | Description                                     | Syntax  |
|--------|--------|----------|-------------------------------------------------|---------|
| 1      | +      | Plus     | Adds two numeric values.                        | a + b   |
| 2      | –      | Minus    | Subtracts right operand from left operand.       | a – b   |
| 3      | *      | Multiply | Multiply two numeric values.                     | a * b   |
| 4      | /      | Divide   | Divide two numeric values.                       | a / b   |
| 5      | %      | Modulus  | Returns the remainder after dividing left operand by the right operand. | a % b   |

  
   # Program for Arithmetic Operator
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
| S. No. | Symbol | Operator | Description | Syntax |
|---|---|---|---|---|
| 1 | < | Less than | Returns true if the left operand is less than the right operand. Else false | a < b |
| 2 | > | Greater than | Returns true if the left operand is greater than the right operand. Else false | a > b |
| 3 | <= | Less than or equal to | Returns true if the left operand is less than or equal to the right operand. Else false | a <= b |
| 4 | >= | Greater than or equal to | Returns true if the left operand is greater than or equal to right operand. Else false | a >= b |
| 5 | == | Equal to | Returns true if both the operands are equal. | a == b |
| 6 | != | Not equal to | Returns true if both the operands are NOT equal. | a != b |

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
  
| Operator    | Symbol | Description                                | Syntax   |
|-------------|--------|--------------------------------------------|----------|
| Logical AND | `&&`   | Returns true if both operands are true.     | `a && b` |
| Logical OR  | `||`   | Returns true if at least one operand is true. | `a || b` |
| Logical NOT | `!`    | Returns the opposite truth value of the operand. | `!a`     |

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
## Assignment Operators
* Assignment operators are used to assign value to a variable.
* These are Assignment Operators :

| S. No. | Symbol | Operator | Description | Syntax |
|---|---|---|---|---|
| 1 | = | Simple Assignment | Assign the value of the right operand to the left operand. | `a = b` |
| 2 | += | Plus and assign | Add the right operand and left operand and assign this value to the left operand. | `a += b` |
| 3 | -= | Minus and assign | Subtract the right operand and left operand and assign this value to the left operand. | `a -= b` |
| 4 | *= | Multiply and assign | Multiply the right operand and left operand and assign this value to the left operand. | `a *= b` |
| 5 | /= | Divide and assign | Divide the left operand with the right operand and assign this value to the left operand. | `a /= b` |
| 6 | %= | Modulus and assign | Assign the remainder in the division of left operand with the right operand to the left operand. | `a %= b` |
				
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
    printf("a %= b: %d\n", a %= b);
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
# Control Statements & Decision Making
* Control statements are the statements which are used to control the flow of execution of the instructions.
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
   ```
#### Output
```
The number is zero.
```
### Switch Statements
* The switch statement in C is a control flow structure that allows the execution of different code blocks based on the value of an expression.
#### Example
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
     #### Syntax of for Loop
   ```
   for (initialization; condition; Increment/decrement) {
    // Code to execute on each iteration
    }
   ```
     #### Example
    ```
    #include <stdio.h>
     int main() {
    // Loop from 0 to 4
    for (int i = 0; i < 5; i++) {
        printf("Number %d\n", i);
      }
    }
    
   ```
### Output

```
Number 0
Number 1
Number 2
Number 3
Number 4
```
### While Loop
* The while loop in C is a control flow statement that allows you to execute a block of code repeatedly as long as a specified condition is true.
  #### Syntax of While Loop
  ```
  while (condition) {
  // code block to be executed
   }
  ```
#### Example
```
#include <stdio.h>
int main() {
    int i = 0;
    // Loop from 0 to 4
    while (i < 5) {
        printf("Number %d\n", i);
        i++; // Increment the loop variable
    }
 }
```
#### Output
```
Number 0
Number 1
Number 2
Number 3
Number 4
```
### do While Loop
* The do-while loop is a control flow statement that allows you to execute a block of code repeatedly as long as a specified condition is true.
* The do-while loop body is executed at least once before the condition is tested.
 ####  Syntax of do While Loop
 ```
 do {
    // Code to execute at least once and then repeatedly while condition is true
  } while (condition);
```
#### Example
```
#include <stdio.h>
int main() {
    int i = 0;
    // Loop that runs as long as i is less than 5
    do {
        printf("Number %d\n", i);
        i++; // Increment the loop variable
    } while (i < 5);
 }
```
#### Output
```
Number 0
Number 1
Number 2
Number 3
Number 4
```
## Jump Statements
* Jump statements in the C programming language allow programmers to alter the normal flow of execution in their code.
* jump Statements are of 3 types
i)   Break
ii)  continue
  ### Break Statements
  * The break statement is used to exit from a loop.
    #### Example
    ```
    #include <stdio.h>
    int main() {
    for (int i = 0; i < 10; i++) {
        if (i == 5) {
            break; // Exit the loop when i equals 5
        }
        printf("%d ", i);
      }
    }
    ```
#### Output
```
0 1 2 3 4
```
### Continue Statements
* The continue statement is used to skip the remaining part of the loop body for the current iteration and proceed with the next iteration of the loop.
  #### Example
  ```
  #include <stdio.h>
   int main() {
    for (int i = 0; i < 10; i++) {
        if (i % 2 == 0) {
            continue; // Skip the rest of the loop body for even numbers
        }
        printf("%d ", i);
    }
    return 0;
  }
  ```
#### Output
```
1 3 5 7 9 
```
# Pointer
* A pointer is a variable that stores the address of another variable.
  ## Syntax of pointer
  ```
  datatype * ptr;
  where,
      ptr is the name of the pointer.
      datatype is the type of data it is pointing to.
  ```
    ## Address Of (&) Operator
* The address of operator '&' returns the address of a variable.
* But, we need to use % to display the address of a variable.
  
  ## Example of Pointer
  ```
  #include <stdio.h>
  int main() {
  int a=6;
  int *ptr;
  ptr=&a;
  printf("The address of variable a is %u\n",ptr);
  printf("The address of variable a is %u\n",*ptr);
    }
``
### Output
```
The address of variable a is 1763721828
The address of variable a is 6
```
 # Array
 * An array is a collection of similar type of elements.
 * It is a simple and fast way of storing multiple values under a single name.
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20230302091959/Arrays-in-C.png" alt="Array" height="350px" width="450px">
    ## Syntax of Array
   ```
   data_type array_name [size1] [size2]...[sizeN];
   ```
   ## Example
   ```
   #include <stdio.h>
   int main() {
   int marks[5];
   for(int i=0;i<5;i++){
     printf("Enter the English marks of students %d :",i+1);
     scanf("%d",&marks[i]);
    }
   }
  ``
## Output
```
Enter the English marks of students 1 :70
Enter the English marks of students 2 :60
Enter the English marks of students 3 :90
Enter the English marks of students 4 :98
Enter the English marks of students 5 :78

=== Code Execution Successful ===
```
# String
* In C, a string is defined as a sequence of characters terminated by a special character called the null character ('\0').
* This null character indicates the end of the string.
  ## Initializing Strings
  * Since string is an array of characters,it can be initialized as follows:
     <img src="https://d8it4huxumps7.cloudfront.net/uploads/images/6492a64d1cd59_strings_in_c_03.jpg" alt="string" height="350px" width="450px">
 ## Printing Strings
 * A string can be printed character by character using printf and %s
      ### Example
      ```
      #include<stdio.h>
      int main(){
      char st[]="hello isha";
      printf("%s",st);
        }
      ```
     
### Output

```
hello isha
```
## gets() and puts()
* gets() is a function which can be used to recieve a multi-word string.
* puts() is a function in a string to the print the output in a newline.
  ### Example
  ```
  #include<stdio.h>
   int main(){
    char s[34];
    printf("Enter your name : ");
    gets(s);
    puts(s);
    printf("Your Name is %s ",s);   
  }
  ```
 ### Output
```
Enter your name : ISHA JANGRA
ISHA JANGRA
Your Name is ISHA JANGRA
```
  # References
 
* https://www.studocu.com/row/document/tribhuvan-vishwavidalaya/information-technology/c-programming-notes/2664815
* https://www.geeksforgeeks.org/operators-in-c/
* https://www.scholarhat.com/tutorial/c/loops-in-c
* https://www.javatpoint.com/c-gets-puts#:~:text=C%20puts()%20function&text=The%20puts()%20function%20is,being%20printed%20on%20the%20console.
