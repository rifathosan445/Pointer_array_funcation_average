# Pointer_array_funcation_average
Write a C program to find the average of the elements of an array .The programe should use a funcation that takes an integer array as input poarameter and returns the average value using a pointer .  


      #include<stdio.h>

     float point(int *ar,int size)//CREATE FUNCATION
    {
    int i,sum=0;
    float *aver;
    for(i=0; i<size; i++)
    {
        sum=sum+*ar;
        ar++;

    }
    float aver2=(float)sum/size ;
    aver=&aver2;
    return *aver;
     }

    int main()//MAIN FUNCATION
    {
    int  a[]= {2,4,6,8,10,11};
    int size=sizeof(a)/sizeof(a[0]);
    float aner=point(a,size);

    printf("%f",aner);

    return 0;
    }
