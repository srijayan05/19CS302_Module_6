# EX 30 C program to add two float elements in an array using realloc() and that array already has three elements.
## DATE: 
## AIM:
To write a C program to add two float elements in an array using realloc() and that array already has three elements.

## Algorithm
1. Start.
2. Declare array size
3. Initialize array elements using malloc()
4. Update array size using realloc()
5. Print the result.
6. End. 

## Program:
```
#include <stdio.h>
#include <stdlib.h>
int main()
 {
    int i;
    float *list;
    list = (float *)malloc(3 * sizeof(float));
    if (list == NULL)
    {
        printf("Initial memory allocation failed.\n");
        return 1;
    }
    list[0] = 12.33;
    list[1] = 67.44;
    list[2] = 89.55;
    list = (float *)realloc(list, 5 * sizeof(float));
    if (list == NULL)
    {
        printf("Memory reallocation failed.\n");
        return 1;
    }
    list[3] = 20.21;
    list[4] = 32.67;
    printf("Result\n");
    for (i = 0; i < 5; i++)
    {
        printf("%.2f ", list[i]);
    }
    printf("\n");
    free(list);
    return 0;
}
```

## Output:
![Screenshot 2025-05-07 110728](https://github.com/user-attachments/assets/9915c07e-a08b-4be1-95df-69579b114302)

## Result:
Thus the program was executed and the output was verified successfully.
