#include <stdio.h>

int main() {
    int n, rev= 0, r, x;

    printf("Enter an integer: ");
    scanf("%d", &n);

    x = n;

    while (n != 0) {
        r = n % 10;
        rev = rev * 10 + r;
        n /= 10;
    }

    if (x == rev) {
        printf("%d is a palindrome.\n", x);
    } else {
        printf("%d is not a palindrome.\n", x);
    }

    return 0;
}