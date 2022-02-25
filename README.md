# implimentation-of-simple-queue
#include<stdio.h>
#include<stdlib.h>
#define MAX 6
int Q[MAX];
int front,rear;
void insert_Q()
{
        int data,ch;

        do{

                if(rear==MAX)
                {
                        printf("queue is full..!!");
                }
                else
                {
                        printf("enter the data:");
                        scanf("%d",&data);
                        Q[rear]=data;
                        rear++;

                }
                printf("1-continue,0-exit");
                scanf("%d",&ch);
        }while(ch==1);
}
void delete_Q()
{
int data;
        if(rear==front)
        {
                printf("queue is full...!!\n");
        }
        else
        {
                printf("deleted element from the queue is:%d");
                Q[front]=data;
                front++;
        }

}
void display()
{
        int i;
        for(i=front;i<rear;i++)
        {
                printf("%d",Q[i]);
        }
}
int main()
{
        int choice=0;
        while(choice<4)
        {
                printf("\noperations on simple queue are \n");
                printf("1.insert \n2.delete \n3.display \n");
                printf("enter your choice:");
                scanf("%d",&choice);
                switch(choice)
                {
                        case 1:
                                insert_Q();
                                break;
                        case 2:
                                delete_Q();
                                break;
                        case 3:
                                display();
                                break;
                        default:
                                printf("check your choice....!\n!");
                }
        }

}


OUTPUT:
operations on simple queue are                                                                        43,14         77%
1.insert                                                                                              44,1          79%
2.delete                                                                                              45,7-14       81%
3.display                                                                                             46,19-26      83%
enter your choice:18C                                                                                 47,2-9        85%
enter the data:1                                                                                      48,12-26      87%
1-continue,0-exit1                                                                                    49,2-9        89%
enter the data:2                                                                                      50,1          91%
1-continue,0-exit1                                                                                    51,10         93%
enter the data:3                                                                                      52,1          95%
1-continue,0-exit1                                                                                    53,14-21      97%
enter the data:4tor command: WQ                                                                       54,16-23      Bot
1-continue,0-exit1
enter the data:5
1-continue,0-exit1
enter the data:6
1-continue,0-exit1
queue is full..!!1-continue,0-exit0

operations on simple queue are
1.insert
2.delete
3.display
enter your choice:3
123456
operations on simple queue are
1.insert
2.delete
3.display
enter your choice:2
operations on simple queue are
1.insert
2.delete
3.display
enter your choice:3
23456
operations on simple queue are
1.insert
2.delete
3.display
enter your choice:2
operations on simple queue are
1.insert
2.delete
3.display
enter your choice:3
3456
enter your choice:4
check your choice....!!

