# unit-change-programe
you can change grams to kg , ml to litr and seconds to hour.

#include <stdio.h>

int main()
{
    float i;
    float num=123;
    printf("Enter the number : ");
    scanf("%f",&i);
    printf("The codes for unit is :\n 1 : grams\n 2 : mililiteres\n 3 : seconds\nEnter the code of unit you want to convert into their respective SI units : \n ");
    scanf("%f",&num);
    
   
        if(num==1){
        num = i/1000;
        printf("The value in kilograms is : %f",num);
        }
        else if(num==2){
        num = i/1000;
        printf("The value in liters is : %f",num);
        }
        else if(num==3){
        num = i/60;
        printf("The value in hours is : %f",num);
        }
        else{
        printf("The choosen unit is invalid\n");
            
        }
    

    return 0;
}
