#include <stdio.h>
int main() {
    int num, originalNum, r, result = 0;
    printf("Enter a number: ");
    scanf("%d", &num);
    originalNum = num;
    while (originalNum != 0) {
        r= originalNum % 10;
        result += r* r* r;
       originalNum /= 10;
    }

    if (result == num)
        printf("%d is an Armstrong number", num);
    else
        printf("%d is not an Armstrong number", num);

    return 0;
}