# 2024090914025-李伊眉-CS-01
## 学习心得与路径
- 学习心得（入门的第一个月）：开学以来才算真正意义上接触了电脑，从不知道怎么换壁纸，找不到win键，不会截屏，不知道要边充边用，不知道用户名要用英文...重学快捷键，复习word...到现在学会了一些基本技能和基础的C编程，终于实现了“半扫盲”，现在想想还是蛮快的。起步过程是痛苦的，什么都不会，搜出来了教程都找不到键，不断感慨自己“怎么什么都不知道”，刚开始用着VS自我感觉良好，开课后慢慢接触VSC也是十分痛苦，先是自己什么都不会试着安装配置（搞崩，求助朋友），不久后出了点问题，同时老师发了教程和压缩包（ok重新装），紧接着运行掉乱码文件夹且改不了路径（求助老师，原来是因为用了中文用户名，差点刷机，ok，新建账户，重装），各种输出乱码，终端闪退（熬夜改），安装wsl后路径又出问题了(ok,VSC再次重装），真是一波五折，折磨我半个月之久的VSC终于没出问题了（暂时）。经历这些后，情绪稳定起来（也可能是被磨平了棱角），生活越来越有目标感和节奏感，开学来有很多事，自己也参加了非常多的活动，所以更加会安排时间（每天晚上整电脑到比高三都晚，难崩），在学习C语言的过程中也有同时推进数学，四级和一堆MOOC，参加面试，竞选班委，开各种会，忙学生组织的事，排练表演三个节目，完成旅游计划，学化妆，甚至还抽时间看了时间简史，真是充实的大学生活！（有点享受了bushi...（srds第一次这么彻彻底底感受学和玩的分离态，爽）
- 路径：B站大学，求助朋友和老师（再次感谢不嫌我蠢的朋友，真的问了好多好多问题），CSDN，百度，C Primer Plus（第六版）
## 问题回答
1. 高级计算机语言与低级计算机语言，各有什么优劣，你更喜欢哪一类计算机语言？
   1. 高级计算机
   - 优点：可读性高，可移植性强，开发效率高，错误检测和处理能力强。
   - 缺点：性能相对较低，对硬件的控制能力不足，资源消耗相对较大。
   2. 低级计算机
   - 优点：执行效率高，对硬件的控制能力强，代码精简。
   - 缺点：可读性差，可移植性差，开发效率低。
   3. 高级计算机语言
      
2. 尝试解读hello.c中每一行的内容。
   - ***#include <stdio.h>*** : #预处理，用于包含标准输入输出头文件，这个头文件中包含了一些用于输入输出操作的函数声明。
   - ***int main()*** : C语言程序的入口。
   - ***printf("Hello, world!");*** : 调用了 printf 函数。
   - ***return 0;*** : 主函数返回一个整数值 0。在C语言中，主函数的返回值通常表示程序的退出状态，返回0表示程序正常结束。
     
3. 删去该程序的哪一行不会影响运行结果？
   - 删去return 0; 不影响运行结果。
     
4. int类型是计算机存储什么元素的方式？为什么main函数要使用int进行声明/定义？
   - 整数类型
   - 这样可以明确地表示main函数返回一个整数值，这个整数值可以被操作系统或其他调用程序用来判断程序的执行状态，使用int类型进行声明可以确保程序在不同的环境中能够正确地与操作系统交互。
     
5. 请调整上述程序的内容，使其输出内容改为Hello glimmer!并附上运行截图
![image](https://github.com/user-attachments/assets/4dc59f4a-6bdc-4eed-9e7b-c8608d339e38)

## 基础语法运用
```
#include <stdio.h>
#include <stdlib.h>
int main() {
    int code;

    printf("Show me your code,please.\n");
    scanf("%d",&code);

    if(code >= 100000 && code <= 999999){
        printf("I am super hacker!");
    }
    else {
        printf("Fake code!");
    }
    system("pause");
    return 0;
}
```

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
