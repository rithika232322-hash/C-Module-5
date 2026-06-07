# Arrays: Matrix Addition in C (Using 2D Arrays)

## 🎯 Aim

To write a C program that adds two matrices using 2-dimensional arrays.

## 🧠 Algorithm

1. **Input**:
   - Read the number of rows and columns.
   - Read elements of Matrix A.
   - Read elements of Matrix B.
2. **Matrix Addition**:
   - Create a third matrix C.
   - For each element `C[i][j]`, compute `C[i][j] = A[i][j] + B[i][j]`.
3. **Output**:
   - Print `"Sum of two matrices:"` followed by elements of Matrix C row by row.

## Progam
```
#include <stdio.h>

int main() {
    int r, c, i, j;
    int A[10][10], B[10][10], C[10][10];
    printf("Enter number of rows and columns: ");
    scanf("%d %d", &r, &c);
    printf("Enter elements of Matrix A:\n");
    for(i = 0; i < r; i++) {
        for(j = 0; j < c; j++) {
            scanf("%d", &A[i][j]);
        }
    }
    printf("Enter elements of Matrix B:\n");
    for(i = 0; i < r; i++) {
        for(j = 0; j < c; j++) {
            scanf("%d", &B[i][j]);
        }
    }
    for(i = 0; i < r; i++) {
        for(j = 0; j < c; j++) {
            C[i][j] = A[i][j] + B[i][j];
        }
    }
    printf("Sum of two matrices:\n");
    for(i = 0; i < r; i++) {
        for(j = 0; j < c; j++) {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```
## Output
<img width="440" height="460" alt="image" src="https://github.com/user-attachments/assets/e75394c7-14ec-4e57-ba4d-edf640d99338" />

## Result
a C program that adds two matrices using 2-dimensional arrays is written.
