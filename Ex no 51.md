# EX 51 C program to reverse a string.
## DATE:
## AIM:
To write a C program to reverse a string.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
C program to reverse a string.
Developed by: 
RegisterNumber:  
*/
#include <stdio.h>
#include <string.h>

int main() {
    char str[100], reversed[100];
    int length, i;

    printf("Enter a string: ");
    scanf("%s", str);  // Reads a single word

    length = strlen(str);

    // Reverse manually
    for (i = 0; i < length; i++) {
        reversed[i] = str[length - i - 1];
    }
    reversed[length] = '\0'; // Null-terminate the reversed string

    printf("Reversed string: %s\n", reversed);
    
    return 0;
}
```

## Output:

<img width="378" height="201" alt="image" src="https://github.com/user-attachments/assets/b87e2e1f-985e-4ccc-ad5b-ee1cba453be7" />


## Result:
Thus the program was executed and the output was verified successfully.
