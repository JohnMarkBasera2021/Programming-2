# Programming-2
#include <stdio.h>
#include <stdlib.h>
#define MAX_LIMIT 10

int main()
{
    char name[MAX_LIMIT];
    int i,age, n, x;
    int num=1;
    const int max_values = 10;
    printf("-------------------------------------\n");
    printf("---------- AGE ELIGIBILITY ----------\n");
    printf("-------------------------------------\n");

    do
    {
        printf("Expected Output %d\n", num);
        //Name
            printf("Name: ");
            scanf("%s", name);
       //%[^\n]s
       // Age
        for(x=0;x<=x;x++)
        {
            printf("Age: ");
            age = scanf("%d", &n);

            if (age == EOF){
                break;
            }
            //if (age != 1) {
            //    puts("Invalid Input. Please Try Again.......");
            //    for (;;)
            //        if (getchar() == '\n')
            //            break;
            //    continue;
            //}

            if ((age != 1)||(n <= 0)) {
                puts("Invalid Input. Please Try Again.......");
                for (;;)
                   if (getchar() == '\n')
                       break;
                continue;
            }
                    if( n >=18 )
                    {
                        printf("You are eligible for voting.\n");
                    }
                    else if(n > 0 && n <18)
                    {
                        printf("You are not eligible for voting.\n");
                    }
            x++;
            break;
        }
    num++;
    printf("\n-------------------------------------\n");
    }while(num<=10);
    return 0;
}
