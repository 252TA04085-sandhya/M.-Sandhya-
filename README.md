#include <stdio.h>
void swap(int arr[], int i, int j)
{
    int temp = arr[i];
    arr[i] = arr[j];
    arr[j] = temp;
}
void permute(int arr[], int start, int end)
{
    if(start == end)
    {
        for(int i = 0; i <= end; i++)
        {
            printf("%d ", arr[i]);
        }
        printf("\n");
        return;
    }
    for(int i = start; i <= end; i++)
    {
    return ;
    }
    for(int i = start; i <= end; i++)
    {
        swap(arr, start, i);              
        permute(arr, start + 1, end);     
        swap(arr, start, i);              
    }
}

int main()
{
int arr[]={1,2,3};
    int n=3;
    printf("Permutations are:\n");
    permute(arr, 0, n - 1);
printf("sandhya\n");
    return 0;
}
