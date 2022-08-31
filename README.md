# Array-C.W.
31.08.2022 Lab Class Works

1st Problem :- Find Average of Array numbers.

#include<stdio.h>
int main()
{

    int n, sum = 0;
    float AV;
    scanf("%d",&n);
    int A[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&A[i]);
        sum = sum + A[i];
    }
    
    AV = (1.00*sum)/n;
    printf("AV = %f",AV);
    
    return 0;
}

2ed Problem :- Find the maximum number of Array

#include<stdio.h>
int main()
{

    int n;
    scanf("%d",&n);
    int a[100];
    int b= a[0];
    int c=0;
    for(int i=1;i<n;++i)
    {
        scanf("%d",&a[i]);
        if(a[i]>b)
        {
            b=a[i];
            c=i;
        }
    }
    printf("%d\n",b);
    printf("%d",c);

}

3rd Problem :- Find a specific number in Array

#include<stdio.h>
int main()
{

    int n,a[100];
    scanf("%d",&n);
    int item=10,i;
    int count=0;
    for (i=0;i<n;++i)
    {
        scanf("%d",&a[i]);
        if(item==a[i])
        {
            count=1;
        }
    }
    if(count==1)
    {
        printf("found\n");
    }
        else
            printf("Not found");
            
    return 0;
}

4th Problem :- Find which which numbers are repeat in the array.

#include<stdio.h>
int main()
{

    int i,j,n,a[100],item;
    scanf("%d",&n);
    for(i=0;i<n;++i)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;++i){
        int flag=0;
        item=a[i];
    for(j=0;j<=i-1;j++)
    {
        if(item==a[j]){flag=1;break;}
    }
    if(flag==0){
        for(j=i+1;j<n;++j)
        {
            if(item==a[j]){
         printf("%d\n",item);
         break;
         }
        }
      }
    }
 return 0;
 
}

