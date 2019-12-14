
# **PROGRAMMING FOR PROBLEM SOLVING**
## NAME-ARSHDEEP SINGH
## ITA1-1921013

# 1.Write a program to convert Centigrate to fahrenheit scale.
```C
#include<stdio.h>
int main()
{
	
	float cen, fah;
	printf("Enter temperature in Celsius : ");
	scanf("%f",&cen);
	fah=(1.8 * cen) + 32;
	printf("\nTemperature in Fahrenheit = %f",fah);
	return 0;
}
```
output of program
```C
Enter the temerature in Celsious : 37
Temperatur in fahrenheit : 98.599998
```
# 2. Write a program to check whether even or odd number .
```C
#include<stdio.h>
int main()
{
    int num;
    printf("Enter any number: ");
    scanf("%d", &num);
    if(num%2 == 0)
        printf("\nIt's an even number.");
    else
        printf("\nIt's an odd number.");
	
    return 0;
}
```
Output of program
```C
Enter any number:6
It's an even number.
```
# 3.Write a program which takes 2 integers operands and one operand from user perform the operator and then print the result (+,-,/,*,%).
```C
#include <stdio.h>
void main()
{
   int a, b, c;
   char ch;
   clrscr() ;
   printf("Enter your operator(+, -, /, *, %)\n");
   scanf("%c", &ch);
   printf("Enter the values of a and b\n");
   scanf("%d%d", &a, &b);

   switch(ch)
   {
      case '+': c = a + b;
        printf("addition of two numbers is %d", c);
        break;
      case '-': c = a - b;
         printf("substraction of two numbers is %d", c);
         break;
      case '*': c = a * b;
         printf("multiplication of two numbers is %d", c);
         break;
      case '/': c = a / b;
         printf("remainder of two numbers is %d", c);
         break;
      case '%': c = a % b;
         printf("quotient of two numbers is %d", c);
         break;
      default: printf("Invalid operator");
         break;
   }
   getch();
}
```
Output of program
```C
Enter you operator(+, -, /, *, %)
+
Enter the values of a and b
1 3
addition of two numbers is 4
```
# 4.Write a source code to check whether the number is positive or negative.
```C
#include <stdio.h> 
int main() 
{ 

    int A; 

 
    printf("Enter the number A: "); 

    scanf("%d", &A); 

  

    if (A > 0) 

        printf("%d is positive.", A); 

    else if (A < 0) 

        printf("%d is negative.", A); 

    return 0; 
} 
```
Output of program
```C

Enter the number A =: -54
-54 is negative.
```
