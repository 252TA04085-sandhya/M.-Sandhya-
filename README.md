#include <stdio.h>

void generateSubsets(int arr[], int n, int index, int subset[], int size) {
    
    if(index == n) {
        printf("{ ");
        for(int i = 0; i < size; i++) {
            printf("%d ", subset[i]);
        }
        printf("}\n");
        return;
    }
    subset[size] = arr[index];
    generateSubsets(arr, n, index + 1, subset, size + 1);

    
    generateSubsets(arr, n, index + 1, subset, size);
}

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n], subset[n];

    printf("Enter elements:\n");
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("\nSubsets are:\n");
    generateSubsets(arr, n, 0, subset, 0);
printf("sandhya\n");
    return 0;
}
