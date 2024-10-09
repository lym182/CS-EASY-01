# CS-EASY-01

## 课后题
```
#include<stdio.h>
//求最大公约数的Euclid算法
int main(void){
    int m,n,t;
    printf("Enter two integers:");
    scanf("%d%d",&m,&n);
    while(n!=0){
        t=m%n;
        m=n;
        n=t;
    }
    printf("Greatest common divisor：%d",m);
    return 0;
}
```
