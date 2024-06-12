# Increasing-Horizontal-and-Vertical-Star-Pattern
Given that the pattern involves a combination of increasing horizontal lines of stars followed by vertical lines of stars, we could call it the "Increasing Rectangular and Vertical Star Pattern."
```c
#include <stdio.h>

int main()
{
    int i, j, k, n;
    printf("Enter the number of stars per line: ");
    scanf("%d", &n);

    for (i = 1; i < 10; i++) {
        // Print horizontal line of stars
        for (j = 1; j <= n * i; j++) {
            printf("*");
        }
        printf("\n");

        // Print vertical lines of stars
        for (k = 0; k < i; k++) {
            printf("*\n");
        }
    }

    return 0;
}
```

### Explanation:

1. **Input Handling:**
   - The user inputs the value `n`, which represents the base number of stars per line.

2. **Outer Loop:**
   - The outer loop `for (i = 1; i < 10; i++)` iterates through the numbers 1 to 9.

3. **Horizontal Stars:**
   - The first inner loop `for (j = 1; j <= n * i; j++)` prints `n * i` stars on a single line.

4. **Vertical Stars:**
   - The second inner loop `for (k = 0; k < i; k++)` prints `i` vertical stars (each star on a new line).

### Output Example:

If the user inputs `3` as the value of `n`, the output will be:

```
***
*
******
*
*
*********
*
*
*
**************
*
*
*
*
*****************
*
*
*
*
*
********************
*
*
*
*
*
*
*************************
*
*
*
*
*
*
*
******************************
*
*
*
*
*
*
*
*
```

This approach prints a rectangular block of stars followed by vertical lines of stars, increasing with each iteration.
