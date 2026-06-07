# Pointers: Reverse a String Using Pointers in C

## 🎯 Aim

To write a C program that prints a string in reverse using a pointer.

## 🧠 Algorithm

1. **Input**: Read a string from the user.
2. **Reverse String**:
   - Use a pointer to traverse the string to find its length.
   - Then, move the pointer to the last character of the string.
   - Print characters in reverse by decrementing the pointer.
3. **Output**: Display the reversed string.

## Program
```
#include <stdio.h>

int main() {
    char str[100];
    char *ptr;
    printf("Enter a string: ");
    scanf("%s", str);
    ptr = str;
    while(*ptr != '\0') {
        ptr++;
    }
    ptr--;
    printf("Reversed string: ");
    while(ptr >= str) {
        printf("%c", *ptr);
        ptr--;
    }

    return 0;
}
```
## Output
<img width="441" height="264" alt="image" src="https://github.com/user-attachments/assets/a443e4b4-41ea-458f-bd7a-d71fce524201" />

## Result
 a C program that prints a string in reverse using a pointer is written.
