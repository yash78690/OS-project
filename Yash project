#include<stdio.h>
#include<unistd.h>
#include<semaphore.h>
void entershop(int left,int right)
{
	int a;
	int c;
	printf("How Many Persons : \n");
	scanf("%d",&a);
	if(a==2)
	{
	    printf("Are they in group -> 1 for Yes or 2 for No : \n");
	    scanf("%d",&c);
	    if(c==1)
	    {
	        printf("Enter In The Shop -> Wait for 5 Seconds\n");
	        sleep(5);
	    }
	    else
	    {
	        printf("Make a Group");
		    entershop(5,5);
	    }
	}
	else
	{
		printf("Wait for a group -> for 5 seconds\n");
		sleep(5);
		entershop(5,5);
	}
}
void shopforawhile()
{
    int b;
    printf("How many Persons Are there in a Shop : \n");
    scanf("%d",&b);
	if(b>=1)
	{
	    printf("Shopping -> Wait for 5 Seconds\n");
	    sleep(5);
	}
	else
	{
	    printf("Shop is vacant\n");
	    entershop(5,5);
	}
	
}
void leaveshop()
{
	printf("Done Shopping\n");
	entershop(5,5);
}
int main()
{
    int z;
    printf("One Left Hand Person and One Right Hand Person -> 1 for Yes or 2 for No :\n");
    scanf("%d",&z);
    if(z==1)
    {
        entershop(5,5);
        shopforawhile();
        leaveshop();
    }
    else
    {
        printf("Find a Group With One Left and With One Right Hand Person\n");
    }
}
