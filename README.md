# c-assignment-2-05-2025
Execute the following programs and create a  document in github with question, code and output and then upload the pdf file generated from github and also give the github link in the submission.

1. Write a c program to print all prime numbers between two limits.
```
#include <stdio.h>

int main() {
    int low, high, i, j, isPrime;

    printf("Enter two numbers: ");
    scanf("%d %d", &low, &high);

    printf("Prime numbers between %d and %d are:\n", low, high);

    for(i = low; i <= high; i++) {
        if(i <= 1) continue;

        isPrime = 1;

        for(j = 2; j <= i/2; j++) {
            if(i % j == 0) {
                isPrime = 0;
                break;
            }
        }

        if(isPrime)
            printf("%d ", i);
    }

    return 0;
}
```
<img width="1919" height="971" alt="image" src="https://github.com/user-attachments/assets/83ea81a7-b68d-4973-839e-fbd9ab1e05da" />

2. Write a c program to count the number of digits in a number.
```
#include <stdio.h>

int main() {
    int num, count = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    if(num == 0) count = 1;

    while(num != 0) {
        num = num / 10;
        count++;
    }

    printf("Number of digits = %d", count);

    return 0;
}
```

<img width="1350" height="754" alt="image" src="https://github.com/user-attachments/assets/a385176a-6f48-4da3-9bb7-f729d62551c0" />

3. Write a c program to print the alphabet S in n x n matrix.
```
#include <stdio.h>

int main() {
    int n, i, j;

    printf("Enter size: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++) {
        for(j = 0; j < n; j++) {
            if(i == 0 || i == n/2 || i == n-1 ||
               (i < n/2 && j == 0) ||
               (i > n/2 && j == n-1)) {
                printf("*");
            } else {
                printf(" ");
            }
        }
        printf("\n");
    }

    return 0;
}
```
<img width="1453" height="899" alt="image" src="https://github.com/user-attachments/assets/6cb468c3-eb3a-4835-8f7b-3ce7629e0555" />



4. Write a c program to print the pyramid pattern. * *** ***** *******
```
#include <stdio.h>

int main() {
    int i, j, n = 4;

    for(i = 1; i <= n; i++) {
        for(j = 1; j <= n - i; j++) {
            printf(" ");
        }
        for(j = 1; j <= (2*i - 1); j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```
<img width="1643" height="861" alt="image" src="https://github.com/user-attachments/assets/af3b6a9f-b100-4777-b27e-42e27274f484" />


5. Write a c program to find GCD of two numbers using loop.
```
#include <stdio.h>

int main() {
    int a, b, i, gcd;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    for(i = 1; i <= a && i <= b; i++) {
        if(a % i == 0 && b % i == 0) {
            gcd = i;
        }
    }

    printf("GCD = %d", gcd);

    return 0;
}
```
<img width="1667" height="946" alt="image" src="https://github.com/user-attachments/assets/ddc3eac7-9e02-44d4-9cd6-5406bddceb0c" />

