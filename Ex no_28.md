# EX 28 C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.
## DATE:
## Aim:
To write a C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.

## Algorithm:
1. Start.
2. Declare enum type
3. Declare all days in a week
4. Print result
5. End
6. 
## Program:
```
#include <stdio.h>
enum weekdays{ Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday};
int main()
{
 enum weekdays today = Wednesday;
 if (today == Wednesday)
 {
    printf("Today is Wednesday.\n");
 }
}
```

## Output:
![Screenshot 2025-05-07 104635](https://github.com/user-attachments/assets/de5f73d8-f386-4293-99f7-c6f877c782e0)



## Result:
Thus the program was executed and the output was verified successfully.
