#include<stdio.h>
int findHCF(int a,int b)
{
if(b==0)
return a;
return findHCF(b,a%b);
}
int main()
{
int a,b;
printf("enter two numbers");
scanf("%d %d",&a,&b);
int h=findHCF(a,b);
int l=(a*b)/h;
printf("HCF=%d\n",h);
printf("LCM=%d\n",l);
printf("sandhya\n");
return 0;
}
