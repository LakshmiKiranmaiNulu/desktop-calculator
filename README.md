# desktop-calculator
#include <stdio.h>  
int main()  
{   char opt;  
    int n1, n2;   
    float res;  
    printf (" Choose an operator(+, -, *, /) \n ");  
    scanf ("%c", &opt);   
    if (opt == '/' )  
    {  
        printf (" Division");  
    }  
    else if (opt == '*')  
    {  
        printf (" Multiplication");  
     }  
    else if (opt == '-')  
    {  
        printf ("Subtraction");  
     }  
        else if (opt == '+')  
    {  
        printf (" Addition");  
     }  
    printf (" \nEnter numbers: ");  
    scanf (" %d %d", &n1,&n2);   
    switch(opt)  
    {  
        case '+':  
            res = n1 + n2; 
            printf (" Addition sol %.2f",res);  
            break;  
        case '-':  
            res = n1 - n2;  
            printf (" Subtraction sol %.2f",res);  
            break;        
        case '*':  
            res = n1 * n2;  
            printf (" Multiplication sol: %.2f",res);  
            break;
        case '/':  
            if (n2 == 0)
            {  
                printf (" \n Divisor cannot be zero. Please enter another value ");  
                scanf ("%d", &n2);        
                }  
            res = n1 / n2;  
            printf (" Division sol %.2f", res);  
            break;  
             default:
            printf (" Something is wrong!! ");               
    }  
    return 0;  
}  
