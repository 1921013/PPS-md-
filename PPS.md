
# **PROGRAMMING FOR PROBLEM SOLVING**
## NAME-ARSHDEEP SINGH
## ITA1-1921013

# 1.Write a programe to convert Centigrate to fahrenheit scale.
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
output of programs 
```C
Enter the temerature in Celsious : 37
Temperatur in fahrenheit : 98.599998
```
