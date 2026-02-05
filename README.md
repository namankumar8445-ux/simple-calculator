#include <stdio.h>
int main()
{
    char operator;
    double num1,num2,result;
    printf("enetr the operator(+,-,/,*):");
    scanf("%c",&operator);
    printf("enter the two numbers:");
    scanf("%lf %lf",&num1,&num2);
    switch(operator){
        case '+':
         result = num1 + num2;
        printf("%.2lf + %.2lf = %.2lf\n",num1,num2,result);
        break;
        case '-':
        result = num1 - num2;
        printf("%.2lf - %.2lf = %.2lf",num1,num2,result);
        break;
        case '*':
        result = num1*num2;
        printf("%.2lf*%.2lf = %.2lf",num1,num2,result);
        break;
        case '/':
        if(num2 != 0.0){
            result = num1/num2;
            printf("%.2lf/%.2lf = %.2lf",num1,num2,result);
        }
        else{
            printf("error! division by zero is not allowed.\n");
        }
        break;
        default:
        printf("error! operator is not correct./n");
    }
    return 0;
}
