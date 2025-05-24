
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```c
#include <stdio.h>
int main()
{
    char ch1, ch2, ch3;
    scanf(" %c", &ch1);
    scanf(" %c", &ch2);
    scanf(" %c", &ch3);
    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5ccf7ab2-d9d0-4fde-80e2-c4a69fb47eb1)

















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```c
#include <stdio.h>
int main()
{
    int A;
    scanf("%d", &A);
    if (A > 0) {
        printf("The number is positive.\n");
    } else {
        printf("The number is not positive.\n");
    }
    return 0;
}
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/feb3a6a0-51cd-4318-a4a5-160dfe22efeb)











# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```c
#include <stdio.h>
int main() 
{
    float a, b, min1;
    float c,d,min2;
    scanf("%f%f", &a,&b);
    scanf("%f%f", &c,&d);
    min1 = a / b;
    min2 =c / d;
    float min = (min1 < min2) ? min1 : min2;
    printf("The minimum number is: %f\n", min);
    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/359541c0-e21b-46b6-97d2-320f91926765)










## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```c
#include <stdio.h>
int main() 
{
    int value;
    scanf("%d", &value);
    if (value == 1) {
        printf("The value is equal to 1.\n");
    }
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/fe9a264a-368b-4d1f-a603-ed81200690ed)








	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```c
#include <stdio.h>
int main() 
{
    int m1, m2, m3, total;
    float percentage;
    scanf("%d %d %d", &m1, &m2, &m3);
    total = m1 + m2 + m3;
    percentage = ((float)total)/ 3.0;
    if (m1 < 35 || m2 < 35 || m3 < 35 || percentage < 35) {
        printf("Result: Fail\n");
    }
    else if (percentage >= 60) {
        printf("Result: First Division\n");
    }
    else if (percentage >= 50) {
        printf("Result: Second Division\n");
    }
    else {
        printf("Result: Pass\n");
    }

    printf("Total Marks = %d\n", total);
    printf("Percentage = %.2f%%\n", percentage);

    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/040fbab7-baee-4e81-a416-87715eeb40ac)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

