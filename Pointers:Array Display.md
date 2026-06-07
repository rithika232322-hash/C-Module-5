# Pointers: Array Input and Display Using Pointers in C

## 🎯 Aim

To write a C program to read and display an array of 6 integer elements using pointers.

---

## 🧠 Algorithm

1. **Start** the program.
2. **Declare** the following:
   - Integer variable `i` for iteration.
   - Integer variable `n` to store the number of elements.
   - Integer array `arr[10]` to hold up to 10 integers.
   - Integer pointer `parr` initialized to point to the base address of array `arr`.
3. **Read** the value of `n` (number of elements to input, e.g., 6).
4. **Loop** from `i = 0` to `i < n`:
   - Use pointer arithmetic to store input values:
     ```c
     scanf("%d", parr + i);
     ```
5. **Loop** again from `i = 0` to `i < n`:
   - Use pointer dereferencing to print each element:
     ```c
     printf("%d ", *(parr + i));
     ```
6. **End** the program.

## Program
```
#include <stdio.h>

int main() {
    int i, n;
    int arr[10];
    int *parr = arr; 
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", parr + i);
    }
    printf("Array elements are:\n");
    for(i = 0; i < n; i++) {
        printf("%d ", *(parr + i));
    }

    return 0;
}
```
## Output
<img width="448" height="339" alt="image" src="https://github.com/user-attachments/assets/1be62635-a813-457b-8ba7-800fde736993" />

## Result
 a C program to read and display an array of 6 integer elements using pointers is written.

