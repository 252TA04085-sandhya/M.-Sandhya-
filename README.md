#include <stdio.h>

int main()
{
    int n1, n2;

    printf("Enter size of array 1: ");
    scanf("%d", &n1);

    int a[n1];

    printf("Enter elements of array 1:\n");
    for(int i = 0; i < n1; i++)
    {
        scanf("%d", &a[i]);
    }

    printf("Enter size of array 2: ");
    scanf("%d", &n2);

    int b[n2];

    printf("Enter elements of array 2:\n");
    for(int i = 0; i < n2; i++)
    {
        scanf("%d", &b[i]);
    }

    int i = 0, j = 0;

    printf("Merged array:\n");
    while(i < n1 && j < n2)
    {
        if(a[i] < b[j])
        {
            printf("%d ", a[i]);
            i++;
        }
        else
        {
            printf("%d ", b[j]);
            j++;
        }
    }
    while(i < n1)
    {
        printf("%d ", a[i]);
        i++;
    }
    while(j < n2)
    {
        printf("%d ", b[j]);
        j++;
    }
 printf("sandhya\n");
    return 0;
}
