include<stdio.h>
int main()
{
int n,key;
printf("enter n");
scanf("%d",&n);
printf("enter elements");
int a[n];
for(int i=0;i<n;i++)
scanf("%d",&a[i]);
printf("enter key");
scanf("%d",&key);
int low=0,high=n-1,f=0;
while(low<=high)
{
int mid=(low+high)/2;
if(a[mid]==key)
{
printf("found at %d",mid);
f=1;break;
}
else if(a[mid]<key)
low=mid+1;
else
high=mid-1;
}
if(f==0)printf("not found");
printf("sandhya\n");
}
