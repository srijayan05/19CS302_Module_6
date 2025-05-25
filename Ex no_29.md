# EX 29 C program to create two float variables using calloc() and find minimum among them.
## DATE: 
## Aim:
To write a C program to create two float variables using calloc() and find minimum among them.

## Algorithm:
1. Start.
2. Initialize two variables value of calloc().
3. Prompt the user to enter values.
4. Read the values using scanf.
5. Find minimum and print result
6. End   

## Program:
```
#include <stdio.h>
#include <stdlib.h>
int main()
{
    float *a, *b;
    a = (float *)calloc(1, sizeof(float));
    b = (float *)calloc(1, sizeof(float));
    if (a == NULL || b == NULL)
    {
        printf("Memory allocation failed.\n");
        return 1;
    }
    printf("Enter first float value: ");
    scanf("%f", a);
    printf("Enter second float value: ");
    scanf("%f", b);
    if (*a < *b)
    {
        printf("Minimum value = %.2f\n", *a);
    }
    else
    {
        printf("Minimum value = %.2f\n", *b);
    }
    free(a);
    free(b);
    return 0;
}
```
## Output:
![Screenshot 2025-05-07 105854](https://github.com/user-attachments/assets/328e2647-2d53-462f-b98a-aea7a77958c0)

## Result:
Thus the program was executed and the output was verified successfully.
