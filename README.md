# CPP
#include <stdio.h>

void printNumbers(int n)
{
    if (n <= 0)
        return;

    printNumbers(n - 1); // Recursive call to print n-1 numbers first
    printf("%d ", n);    // Print the current number
}

int main()
{
    int n;

    printf("Enter the value of n: ");
    scanf("%d", &n);

    printf("The first %d numbers are: ", n);
    printNumbers(n);

    return 0;
}
