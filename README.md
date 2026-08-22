#include<stdio.h>
int main()
{
int n,i,key;
printf("enter number of array");
scanf("%d",&n);
int a[n];
for(i=0;i<n;i++)
scanf("%d",&a[i]);
scanf("%d",&key);
int f=0;
for(i=0;i<n;i++)
{
if(a[i]==key)
{
f=1;
printf("found at %d",i);
break;
}
}
if(f==0)printf("not found");
printf("sandhya\n");
}
