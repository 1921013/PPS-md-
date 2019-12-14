
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
# 5.Write a source code to find the total experience of the employees.
```C
#include<stdio.h>
int main()
{
int c;
int a,b;
printf("enter no. of employees:");
scanf("%d",&a);
printf("enter their experience:");
scanf("%d",&b);
for(int i=1;i<=a;i++)
{
c+=b;
}
printf("total experience:%d",c);
}
```
Output of program

# 6.Write a program to display the table of user choice.
```C
#include<stdio.h>
int main()
{
    int num, i, tab;
    printf("Enter the number: ");
    scanf("%d", &num);
    printf("\nTable of %d is:\n", num);
    for(i=1; i<=10; i++)
    {
        tab = num*i;
        printf("%d * %2d = %2d\n", num, i, tab);
    }
    getch();
    return 0;
}
```
Output of program
```C
Enter an integer: 9
9 * 1 = 9
9 * 2 = 18
9 * 3 = 27
9 * 4 = 36
9 * 5 = 45
9 * 6 = 54
9 * 7 = 63
9 * 8 = 72
9 * 9 = 81
9 * 10 = 90
```
# 7.Write a program to display the table between the range.
```C
#include <stdio.h>
int main() {
    int n, i, range;
    printf("Enter an integer: ");
    scanf("%d", &n);
    printf("Enter the range: ");
    scanf("%d", &range);
    for (i = 1; i <= range; ++i) {
        printf("%d * %d = %d \n", n, i, n * i);
    }
    return 0;
}
```
Output of program
```C

Enter an integer: 12
Enter the range: 8
12 * 1 = 12 
12 * 2 = 24 
12 * 3 = 36 
12 * 4 = 48 
12 * 5 = 60 
12 * 6 = 72 
12 * 7 = 84 
12 * 8 = 96 
```
# 8.Write a program to check whether the number is prime or not.
```C
#include <stdio.h>
void main()
{
int x=0,i,n;
printf("enter number ");
scanf("%d",&i);
for(n=1;n<=i;n++)
{
if(i%n==0)
x++;
}
if(x==2)
{
printf("no is prime\n");
}
else
{
printf("no is not prime\n");
}
}
```
Output of program
```C
enter number 11
no is prime
```
# 9.Write a program to find the factorial of a number.
```C
#include <stdio.h>
void main()
{
        int a,n=1,i;
        printf("Enter a no");
        scanf("%d",&i);
        for(a=1;a<=i;a++)
        n=n*a;
        printf("factorial of a is %d \n",n);
}
```
OUTPUT
```C
Enter a no 6
factorial of 6 is 720   
```
# 10.Write a program to find factorial of a number using recursion.
```C
#include <stdio.h>
int factorial(int);
int main()
{
        int n,f;
        printf("enter the number ");
        scanf("%d",&n);
        if(n<0)
        printf("factorial is not defined");
        else
        {
                f=factorial(n);
                printf("factorial of number is %d\n",f);
        }
return 0;
}                                                                         
int factorial(int n)
{
        if(n==1)
        return 1;
        else                                                              
        return (n*factorial(n-1));
}
```
OUTPUT
```C
enter the number 5
factorial of number is 120
```
