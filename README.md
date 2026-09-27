# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
2. Implementation of different categories of operators.
# Ex.No:1
## Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
## Algorithm:
Step 1: Start<br>
Step 2: Include the standard input-output library: #include<stdio.h>.<br>
Step 3: Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof():<br>
   3.1 Integer literal (e.g., 10) using `%d`<br>
   3.2 Float literal (e.g., 3.14) using `%f`<br>
   3.3 Character literal (e.g., 'A') using `%c`<br>
   3.4 String literal (e.g., "Hello C") using `%s`<br>
Step 4: Stop<br>
## Program:
```
#include <stdio.h>

int main() {
    printf("Integer literal 10, size: %d bytes\n", (int)sizeof(10));
    printf("Float literal 3.14, size: %d bytes\n", (int)sizeof(3.14));
    printf("Character literal 'A', size: %d bytes\n", (int)sizeof('A'));
    printf("String literal \"Hello C\", size: %d bytes\n", (int)sizeof("Hello C"));

    return 0;
}
```
## Output:
<img width="421" height="110" alt="image" src="https://github.com/user-attachments/assets/b8e12a4b-fd8d-43e1-b97b-37d23b437930" />

## Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
## Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
## Algorithm:
Step 1: Start  <br>
Step 2: Include the standard input-output library: #include<stdio.h>.<br>
Step 3: Define a macro constant `PI` with value `3.14159` using `#define`.<br>
Step 4: Inside `main()`:<br>
   4.1 Declare a constant integer variable `DAYS`<br>
   4.2 Initialize it with the value `7`<br>
Step 5: Use `printf()` to display the values of `PI` and `DAYS`.     <br>
Step 6: Stop<br>
## Program:
```
#include <stdio.h>
#define PI 3.14159   

int main() {
    const int DAYS = 7;   

    // Display values
    printf("Value of PI: %f\n", PI);
    printf("Value of DAYS: %d\n", DAYS);

    return 0;
}
```
## Output:
<img width="231" height="52" alt="image" src="https://github.com/user-attachments/assets/f698787d-964d-4a0e-9cc0-fc3d330c42ea" />

## Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
## Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
## Algorithm:
Step 1: Start<br>
Step 2: Include the standard input-output library: #include<stdio.h>.<br>
Step 3: Inside main(), declare and initialize variables of types int, float, double, and char.<br>
Step 4: Display their values using printf().<br>
Step 5: Stop<br>
## Program:
```
#include <stdio.h>

int main() {
    int num = 10;
    float f = 3.14f;
    double d = 25.6789;
    char c = 'A';

    printf("Integer value: %d\n", num);
    printf("Float value: %f\n", f);
    printf("Double value: %lf\n", d);
    printf("Character value: %c\n", c);

    return 0;
}
```
## Output:
<img width="253" height="110" alt="image" src="https://github.com/user-attachments/assets/11c2ae70-3073-438c-be7a-b2786c286ea3" />
## Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
## Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
## Algorithm:
Step 1: Start<br>
Step 2: Include the standard input-output library: #include<stdio.h>.<br>
Step 3: Declare two integer variables a and b.<br>
Step 4: Prompt the user to enter two integers and read the input using scanf().<br>
Step 5: Perform arithmetic operations on a and b:<br>
   Sum (a + b)<br>
   Difference (a - b)<br>
   Product (a * b)<br>
   Quotient (a / b)<br>
   Remainder (a % b)<br>
Step 6: Perform bitwise operations on a and b:<br>
   AND (a &amp; b)<br>
   OR (a | b)<br>
   XOR (a ^ b)<br>
   Left shift (a << b)<br>
   Right shift (a >> b)<br>
   Bitwise NOT of a (~a) and b (~b)<br>
Step 7: Display the results of all operations using printf().<br>
Step 8: Stop<br>
## Program:
```
#include <stdio.h>

int main() {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    printf("\nArithmetic Operations:\n");
    printf("Sum = %d\n", a + b);
    printf("Difference = %d\n", a - b);
    printf("Product = %d\n", a * b);
    printf("Quotient = %d\n", a / b);
    printf("Remainder = %d\n", a % b);
    printf("\nBitwise Operations:\n");
    printf("AND = %d\n", a & b);
    printf("OR = %d\n", a | b);
    printf("XOR = %d\n", a ^ b);
    printf("Left shift (a << b) = %d\n", a << b);
    printf("Right shift (a >> b) = %d\n", a >> b);
    printf("Bitwise NOT of a = %d\n", ~a);
    printf("Bitwise NOT of b = %d\n", ~b);

    return 0;
}
```
## Output:
<img width="324" height="498" alt="image" src="https://github.com/user-attachments/assets/68912f0e-e244-401e-9379-fc918f6f69d0" />

## Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
## Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
## Algorithm:
Step 1: Start<br>
Step 2: Include the standard input-output library: #include<stdio.h>.<br>
Step 3: Input a character ch from the user.<br>
Step 4: Check if ch is a digit ('0' to '9').<br>
   If true → Print "Digit" → Go to Step 8.<br>
   If false → Go to Step 5.<br>
Step 5: Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').<br>
   If true → Go to Step 6.<br>
   If false → Go to Step 7.<br>
Step 6: Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).<br>
   If true → Print "Vowel" → Go to Step 8.<br>
   If false → Print "Consonant" → Go to Step 8.<br>
Step 7: Print "Special Symbol".<br>
Step 8: Stop<br>
## Program:
```
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);
    if (ch >= '0' && ch <= '9') {
        printf("Digit\n");
    }
    else if ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) {
        if (ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
            ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') {
            printf("Vowel\n");
        } else {
            printf("Consonant\n");
        }
    }
    
    else {
        printf("Special Symbol\n");
    }

    return 0;
}
```
## Output:
<img width="225" height="54" alt="image" src="https://github.com/user-attachments/assets/68a8dd95-425c-49bc-ba1f-9cc8b4fb6dfa" />

## Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.
