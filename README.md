int main()
{
    int a[10],n,i;
    scanf("%d",&n);
    int tempA=n;
    for(i=0;n>0;i++)
    {
       a[i]=n%2;
       n=n/2;
    }
    for(i=1;i>=0;i++)
     
     printf("%d",a[i]);
     printf(" ");
     int octal[100];
     int tempB = tempA;
     i=1;
     while(tempA!=0)
      {
          octal[i++]=tempA % 8;
          tempA = tempA/8;
      }
      
      for (int j=i-1;j>0;j--)
         printf("%d",octal[j]);
        printf(" ");
        char hexa[100];
        i=0;
    
        while(tempB!=0)
        {
             int r = tempB%16;
                if(r<10)
            
                hexa[i++]=48+r;
                
                else
                hexa[i++]=55+r;
                tempB=tempB/16;
            
        }
        
     
       for(int j=i-1;j>=0;j--)
       printf("%c",hexa[j]);
     }
       
