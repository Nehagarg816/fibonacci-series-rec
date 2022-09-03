# fibonacci-series-rec
This is a program for calculation of fibonacci series using recursion in functions in C programming.
#include <stdio.h>
int fib(int a);

int main()
{
    int a;
    printf("Enter the number of which series is required:");
    scanf("%d",&a);
    int s;
    s = fib(a);
    printf("Fibonacci series of entered number is %d",s);
    return 0;
}
int fib(int x)
{
    int series;
    if(x==0)
    {
        return 0;
    }
    else if (x == 1 || x == 2)
    {
        return 1;
    }
    else
    {
        series = fib(x - 1) + fib(x - 2);
    }
    return (series);
}
