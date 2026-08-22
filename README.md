#include<stdio.h>
int main()
{
int n;
printf("enter number of terms");
scanf("%d",&n);
int a=0 ,b=1,c;
printf("Fibonacci series:/n");
for(int i=1;i<=n;i++)
{
printf("%d",a);
c=a+b;
a=b;
b=c;
}
printf("sandhya\n");
return 0;
}
