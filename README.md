#include <stdio.h>
int isPrime(int n) {
    if (n <= 1)
        return 0;
    for (int i = 2; i <= n / 2; i++) {
        if (n % i == 0)
            return 0;
    }
    return 1;
}

int main() {
    int n;

    printf("Enter number: ");
    scanf("%d", &n);
    if (isPrime(n))
        printf("Prime number\n");
    else
        printf("Not a prime number\n");
printf("sandhya\n");
    return 0;
}
