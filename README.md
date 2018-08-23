#include<stdio.h>
#include<String.h>
int main() 
{
    int ch;
    printf("Welcome to Management System Application\n");

 
        
            int nstu;
            printf("Enter the no of students");
            scanf("%d\n",&nstu);
            char name[nstu],branch[nstu];
            int age[nstu],year[nstu],sem[nstu];
            float sem_score[nstu];
            for(int i=0;i<nstu;i++)
            {
                printf("Enter name\n");
                scanf("%c\n",name[i]);
                printf("enter age\n");
                scanf("%d\n",age[i]);
                printf("branch and year and sem\n");
                scanf("%c %d %d\n",branch[i],&year[i],&sem[i]);
                printf("Enter the previous semister score\n");
                scanf("%f\n",&sem_score[i]);
            }
                
       
            
                printf("The list of the Students are following :\n");
                for(int i=0;i<nstu;i++)
                {
                    printf("Student %d\n",i+1);
                    printf("Name : %s",name[i]);
                    printf("Age : %d\n",age[i]);
                    printf(" Branch : %s",branch[i]);
                    printf(" year and sem : %d %d\n",year[i],sem[i]);
                    printf("Sem Score percentage: %0.2f\n",sem_score[i]);
                    
                    
                }
                float cutoff;
                scanf("%f",&cutoff);
                char cmp[100];
                scanf("%c",cmp);
                if(cmp=="greater")
                
                {
                
                for(int i=0;i<nstu;i++)
                {
                    if(sem_score[i]>cutoff)
                    {
                        
                        printf("Student %d\n",i+1);
                    printf("Name : %s",name[i]);
                    printf("Age : %d\n",age[i]);
                    printf(" Branch : %s",branch[i]);
                    printf(" year and sem : %d %d\n",year[i],sem[i]);
                    printf("Sem Score percentage: %0.2f\n",sem_score[i]);
                    }
                }
                }
             else if(cmp=="less than")
                
                {
                
                for(int i=0;i<nstu;i++)
                {
                    if(sem_score[i]<cutoff)
                    {
                        
                        printf("Student %d\n",i+1);
                    printf("Name : %s",name[i]);
                    printf("Age : %d\n",age[i]);
                    printf(" Branch : %s",branch[i]);
                    printf(" year and sem : %d %d\n",year[i],sem[i]);
                    printf("Sem Score percentage: %0.2f\n",sem_score[i]);
                    }
                }
            }
            else
            {
                for(int i=0;i<nstu;i++)
                {
                    if(sem_score[i]==cutoff)
                    {
                        
                       printf("Student %d\n",i+1);
                    printf("Name : %s",name[i]);
                    printf("Age : %d\n",age[i]);
                    printf(" Branch : %s",branch[i]);
                    printf(" year and sem : %d %d\n",year[i],sem[i]);
                    printf("Sem Score percentage: %0.2f\n",sem_score[i]);
                    }
                }
            }
            
        
    
    return 0;
    

}
