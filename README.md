# S.Sai-Saranya-C-program
ASSIGNMENT
1.
#include <stdio.h>
int main()
{
    int arr[]={6,12,18,24};
    int x=0;
    x=arr[1]+(arr[1]=2);
    printf ("%d",x);
    return 0;
}

![image](https://user-images.githubusercontent.com/125387475/226937867-5b9104c4-9f71-42e1-a059-f4962f60c173.png)
output :14 
 
 2.
#include <stdio.h>
#include <conio.h>
void main(){
        int i=3,val;
        val = sizeof f(i)+ +f(i=1)+ +f(i-1);
        printf ("%d %d",val,i);
    }
    int f(int num){
        return num*5;
    }
![image](https://user-images.githubusercontent.com/125387475/226938111-6d6a651b-a983-469b-9384-01f13e6656f3.png)
out put:9  1


3.
#include<stdio.h>
#include<conio.h>
float avg(float,float,float);
void main(){
    float p=1,q=2,r=-2,a;
    a=avg(p,(q=4,r=-12,q),r);
    printf("%f",a);  
}
float avg(float x,float y,float z){
    return (x+y+z)/3;
}


output:-2.33333

4.
void main()
{
int const *p=5;
printf("%d",++*p);
}



5.
#include <stdio.h>
void main()
{
int c[ ]={2.8,3.4,4,6.7,5};
int j,*p=c,*q=c;
for(j=0;j<5;j++) {
printf(" %d ",*c);
++q; }
for(j=0;j<5;j++){
printf(" %d ",*p);
++p; }
}



6.
#include <stdio.h>
void main()
{
char string[]="Hello World";
display(string);
}
void display(char *string)
{
printf("%s",string);
}



7.
#include <stdio.h>
using namespace std;
  
void display()
{
      
    int n = 5;
    int space = n / 2, num = 1;
       
   
    for (int i = 1; i <= n; i++)
    {
        
        for (int j = 1; j <= space; j++)            
            cout<<" ";
           
        
        int count = num / 2 + 1;
          
        for (int k = 1; k <= num; k++)
        {
            cout<<count;
              
            
            if (k <= num /2 )
                count--;
  
           
            else
                count++;
        }
  
        cout<<"\n";
  
       
        if (i <= n / 2)
        {
            space = space - 1;
            num = num + 2;
        }
  
       
        else
        {
            space = space + 1;
            num = num - 2;
        }
    }
}
  

int main()
{
display();
return 0;
}



8.
include <stdio.h>
using namespace std;
 
int findFirst(int arr[], int n, int x)
{
    sort(arr, arr + n);
 
    
    int* ptr = lower_bound(arr, arr + n, x);
 
   
    return (*ptr != x) ? -1 : (ptr - arr);
}
 
int main()
{
    int x = 20, arr[] = { 10, 30, 20, 50, 20 };
    int n = sizeof(arr) / sizeof(arr[0]);
    cout << findFirst(arr, n, x);
    return 0;
}




9.
#include "string.h"
typedef struct stu1{
    char name1[6];
    char name2[6];
    double marks;
}STU1;
void main(){
    STU1 s1={"rohit","kumar",87.43},*p1;
    char *p;
    p1=&s1;
    p=memchr(p1,'u',sizeof(STU1));
    printf("%s",p);  
}
  output:umar
  
  

10.#define square(x) x*x
main()
{
int i;
i = 64/square(4);
printf("%d",i);
}









