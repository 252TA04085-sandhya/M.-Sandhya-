#include <stdio.h>

int main() {
    int n, i, j;
    float marks[5], total, avg;
    char grade;

    printf("Enter number of students: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        printf("\n--- Student %d ---\n", i);

        total = 0;

        // Input marks for 5 subjects
        for (j = 0; j < 5; j++) {
            printf("Enter marks for subject %d: ", j + 1);
            scanf("%f", &marks[j]);
            total += marks[j];
        }

        // Calculate average
        avg = total / 5;

        // Grade assignment
        if (avg >= 90)
            grade = 'A';
        else if (avg >= 80)
            grade = 'B';
        else if (avg >= 70)
            grade = 'C';
        else
            grade = 'D';   // Below 70

        // Display result
        printf("\nTotal Marks = %.2f", total);
        printf("\nAverage Marks = %.2f", avg);
        printf("\nGrade = %c\n", grade);
    }

    return 0;
}
