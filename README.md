include <stdio.h>
int main()
{
int n;
    printf("Enter number of terms: ");
    scanf("%d", &n);
int a=0,b=1,c;
        printf("Nth Fibonacci");
    for(int i=1;i<n;i++)
    {
            c = a + b;
            a = b;
            b = c;
        printf("%d",a);
        printf("sandhya\n");
    }
    return 0;
}
