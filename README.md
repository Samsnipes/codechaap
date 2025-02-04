BIT WISE OPS
#include <stdio.h>

int main() {
    int choice, num1, num2, result, shift;
    do {
        
        printf("\nMenu:\n");
        printf("1. Bitwise AND\n");
        printf("2. Bitwise OR\n");
        printf("3. Right Shift\n");
        printf("4. Left Shift\n");
        printf("5. Exit\n");
        printf("Enter your choice: "); 

        scanf("%d", &choice);

        switch (choice) {
            case 1:
                printf("Enter two integers: ");
                scanf("%d %d", &num1, &num2);
                result = num1 & num2;
                printf("Result of Bitwise AND: %d\n", result);
                break;
            case 2:
                printf("Enter two integers: ");
                scanf("%d %d", &num1, &num2);
                result = num1 | num2;
                printf("Result of Bitwise OR: %d\n", result);
                break;
            case 3:
                printf("Enter an integer and shift value: ");
                scanf("%d %d", &num1, &shift);
                result = num1 >> shift;
                printf("Result of Right Shift: %d\n", result);
                break;
            case 4:
                printf("Enter an integer and shift value: ");
                scanf("%d %d", &num1, &shift);
                result = num1 << shift;
                printf("Result of Left Shift: %d\n", result);
                break;
            case 5:                 printf("Exiting program.\n");
                break;
            default:
                printf("Invalid choice. Please try again.\n");         }
    } while (choice != 5);
    return 0; }
