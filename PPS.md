
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
```c
enter no. of employees:50
enter their experience:15
total experience:750
```

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
# 11.Write a program to check whether the number is prime or not between the range.
```C
#include <stdio.h>
int main() 
{
    int low, high, i, flag;
    printf("Enter two numbers(intervals): ");
    scanf("%d %d", &low, &high);
    printf("Prime numbers between %d and %d are: ", low, high);
    while (low < high) {
        flag = 0;
        // if low is a non-prime number, flag will be 1
        for (i = 2; i <= low / 2; ++i) {
            if (low % i == 0) {
                flag = 1;
                break;
            }
        }
        if (flag == 0)
            printf("%d ", low);
        ++low;
    }
    return 0;
}
```
Output of program
```C

Enter two numbers(intervals): 20 
50
Prime numbers between 20 and 50 are: 23 29 31 37 41 43 47
```
# 12.Write a program to find greater number in an array.
```C
#include <stdio.h>
 
int main()
{
 
        int array[50], size, i, largest;
 
        printf("\n Enter the size of the array: ");
	scanf("%d", &size);
 
        printf("\n Enter %d elements of  the array: ", size);
 
        for (i = 0; i < size; i++)
		scanf("%d", &array[i]);
 
        largest = array[0];
 
        for (i = 1; i < size; i++) 
        {
		if (largest < array[i])
			largest = array[i];
	}
 
        printf("\n largest element present in the given array is : %d", largest);
 
        return 0;
 
}
```
Output of program
```C
Enter the size of the array: 5
 
Enter 5 elements of  the array: 12
56
34
78
100
 
largest element present in the given array is : 100
```
# 13.Write a program to reverse a number.
```C
#include <stdio.h>
void main()
{
        int a,n,r=0;
        printf("enter number");
        scanf("%d",&n);
        while(n>0)
        {
                a=n%10;
                r=r*10+a;
                n=n/10;
        }
        printf("reverse no is %d \n",r);
}
```
OUTPUT
```C
enter number 461 
reverse no is 164
```
# 14. programs to find out the average of 4 integers with array
```C
#include <stdio.h>
int main()
{
    int avg = 0;
    int sum =0;
    int x=0;

    int num[4];

    for (x=0; x<4;x++)
    {
        printf("Enter number %d \n", (x+1));
        scanf("%d", &num[x]);
    }
    for (x=0; x<4;x++)
    {
        sum = sum+num[x];
    }

    avg = sum/4;
    printf("Average of entered number is: %d", avg);
    return 0;
}
```
output 
```C
Enter number 1 
10
Enter number 2 
10
Enter number 3 
20
Enter number 4 
40
Average of entered number is: 20
```
# 15.Write a program to print simple matrix in array.
```C
#include <stdio.h>
int main() {
  int values[5];
  printf("Enter 5 integers: ");
  
  for(int i = 0; i < 5; ++i) {
     scanf("%d", &values[i]);
  }
  printf("Displaying integer");
  for(int i = 0; i < 5; ++i) {
     printf("%d\n", values[i]);
  }
  return 0;
}
```
Output of program
```C
Enter 5 integers: 1
-3
34
0
3
Displaying integers: 1
-3
34
0
3
```
