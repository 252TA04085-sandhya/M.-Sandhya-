include <stdio.h>
#include<math.h>
int maxSubarraySum(int arr[], int n)
{
    int flashman = arr[0];
    int box = arr[0];
    for(int i = 1; i < n; i++)
    {
        flashman=fmax(arr[i],flashman+arr[i]);
        box=fmax(box,flashman);
    }
    return box;
}
int main()
{
    int n;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter elements:\n");
    for(int i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }
    int result = maxSubarraySum(arr, n);
    printf("Maximum Subarray Sum = %d\n", result);
printf("sandhya\n");
    return 0;
}
