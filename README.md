# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  

# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
#include <stdio.h>

int main()
{
    
    printf("Integer literal: %d, Size: %zu bytes\n", 10, sizeof(10));


    printf("Float literal: %f, Size: %zu bytes\n", 3.14f, sizeof(3.14f));

    
    printf("Character literal: %c, Size: %zu bytes\n", 'A', sizeof('A'));

    
    printf("String literal: %s, Size: %zu bytes\n", "Hello C", sizeof("Hello C"));

    return 0;
}

# Output:
<img width="453" height="147" alt="image" src="https://github.com/user-attachments/assets/3e71aed3-bc56-484a-96d7-36c69c833535" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.

# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
#include <stdio.h>

/* Macro constants */
#define PI 3.14
#define MAX 100

int main()
{
  
    const int age = 20;
    const float gravity = 9.8;

    printf("Macro constant PI = %.2f\n", PI);
    printf("Macro constant MAX = %d\n", MAX);

    printf("Constant variable age = %d\n", age);
    printf("Constant variable gravity = %.1f\n", gravity);

    return 0;
}

# Output:
<img width="405" height="151" alt="image" src="https://github.com/user-attachments/assets/5b1c30f8-0f67-4871-9507-a1a68642f20f" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
#include <stdio.h>

int main()
{
    int a = 10;
    float b = 3.14f;
    double c = 123.456789;
    char d = 'A';

    printf("Integer value: %d\n", a);
    printf("Float value: %f\n", b);
    printf("Double value: %lf\n", c);
    printf("Character value: %c\n", d);

    return 0;
}

# Output:
<img width="515" height="163" alt="image" src="https://github.com/user-attachments/assets/efa8ab61-0dea-4266-b1b9-1bf9aba46b7e" />

# Result: 
Hence the program was implemented and executed successfully and the required output was obtained. 
# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shit, and NOT.
 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
#include <stdio.h>

int main()
{
    int a, b;


    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    
    printf("\nArithmetic Operations:\n");
    printf("Addition: %d + %d = %d\n", a, b, a + b);
    printf("Subtraction: %d - %d = %d\n", a, b, a - b);
    printf("Multiplication: %d * %d = %d\n", a, b, a * b);

    if (b != 0)
    {
        printf("Division: %d / %d = %d\n", a, b, a / b);
        printf("Remainder: %d %% %d = %d\n", a, b, a % b);
    }
    else
    {
        printf("Division and Remainder not possible (division by zero)\n");
    }

    
    printf("\nBitwise Operations:\n");
    printf("AND: %d & %d = %d\n", a, b, a & b);
    printf("OR: %d | %d = %d\n", a, b, a | b);
    printf("XOR: %d ^ %d = %d\n", a, b, a ^ b);
    printf("Left Shift: %d << 1 = %d\n", a, a << 1);
    printf("NOT of %d = %d\n", a, ~a);

    return 0;
}

# Output:
<img width="567" height="531" alt="image" src="https://github.com/user-attachments/assets/a416286e-2c1d-48e2-baf2-6ed372d4c691" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5 Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.

 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
#include <stdio.h>

int main()
{
    char ch;

    printf("Enter a character: ");
    scanf(" %c", &ch);   

    
    (ch >= '0' && ch <= '9') ?
        printf("'%c' is a Digit\n", ch) :
    ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ?
        ((ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
          ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ?
            printf("'%c' is a Vowel\n", ch) :
            printf("'%c' is a Consonant\n", ch)) :
        printf("'%c' is a Special Symbol\n", ch);

    return 0;
}

# Output:
<img width="284" height="233" alt="image" src="https://github.com/user-attachments/assets/4d8ef97e-ba07-42a3-b5f9-d47fcc49a5d4" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


