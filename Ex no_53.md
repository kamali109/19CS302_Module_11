# EX 53 C program to remove duplicates in an array.
## DATE:
## AIM:
To write a C program to remove duplicates in an array.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
C program to remove duplicates in an array
Developed by: KAMALI.S
RegisterNumber:  212222060109
*/
#include <stdio.h>

void removeDuplicates(int arr[], int *n) {
    int temp[*n];
    int index = 0;

    for (int i = 0; i < *n; i++) {
        int duplicate = 0;
        for (int j = 0; j < index; j++) {
            if (arr[i] == temp[j]) {
                duplicate = 1;
                break;
            }
        }
        if (!duplicate) {
            temp[index++] = arr[i];
        }
    }

    for (int i = 0; i < index; i++) {
        arr[i] = temp[i];
    }

    *n = index;
}

int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter the elements: ");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    removeDuplicates(arr, &n);

    printf("Array after removing duplicates: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    
    return 0;
}
```

## Output:

<img width="455" height="251" alt="image" src="https://github.com/user-attachments/assets/4d97d32e-1877-41dd-bf9b-832b3bb78dcf" />
## Result:
Thus the program was executed and the output was verified successfully.
