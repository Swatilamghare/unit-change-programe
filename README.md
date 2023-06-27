# unit-change-programe

   #include <stdio.h>

int main()
{
    int num=012345;
    double i;
    /*1 = km to miles
    2 = inches to foot 
    3 = cm to inches
    4 = inches to meters
    5 = pound to kg*/
    
    
    printf("The codes for available conversions are as follows : \n0 = To end the programe\n1 = km to miles\n2 = inches to foot\n3 = cm to inches\n4 = inches to meters\n5 = pound to kg \n");
    
    for(num=1;num<6;){
        printf("Enter the code for the conversion you want : ");
        scanf("%d",&num);
        
        if(num==0){
            printf("Are you sure you want to end the programe?\n If 'yes' press any number or character : ");
            scanf("%d",&num);
            break;
        }
        else if(num==1){
            printf("Enter the number you want to convert in miles : ");
            scanf("%lf",&i);
            printf("%lf kms = %lf miles\n",i,i* 0.62137119);
            continue;
        }
        else if(num==2){
            printf("Enter the number you want to convert in foot : ");
            scanf("%lf",&i);
            printf("%lf cm = %lf foot\n",i,i/12);
            continue;
        }
        else if(num==3){
            printf("Enter the number you want to convert in inches : ");
            scanf("%lf",&i);
            printf("%lf inches = %lf inches\n",i,i*0.393701);
            continue;
        }
        else if(num==4){
            printf("Enter the number you want to convert in meters : ");
            scanf("%lf",&i);
            printf("%lf inches = %lf meters\n",i,i*0.0254);
            continue;
        }
        else if(num==5){
            printf("Enter the number you want to convert in kgs : ");
            scanf("%lf",&i);
            printf("%lf pound = %lf kgs\n",i,i* 0.45359237);
            continue;
        }
     
        else{
            printf("Oops!! You have choosen invalid conversion code.Please try again.\n");
            continue;
        }
        
    }
    
    
    return 0;
}
   
