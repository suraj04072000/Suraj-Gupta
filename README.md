#include <stdio.h>

int main()
{
    char oprator;
    double num1, num2, result;
    // Take oprator input
    printf("Enter the oprator (+,-,*,/):");
    scanf("%c", &oprator);
    // take number input
    printf("Enter the two number:\n ");
    scanf("%lf %lf", &num1, &num2);
// perform the calculation using swich
switch (oprator)
{
    case '+':
    result = num1 + num2;
    printf("result :%lf\n", result);
    break;
case '-':
    result = num1 - num2;
    printf("result :%.2lf\n", result);
    break;
case '*':
    result = num1 * num2;
    printf("result :%.2lf\n", result);
    break;
case '/':
    if (num2 !=0)
    {
       result = num1 / num2;
       printf("result : %.2lf\n",result);
    } else{
        printf("error : Division by zero is not allowed.\n");
    }
    break;

default:
    printf("invaild oprator\n");
}

    return 0;
}
