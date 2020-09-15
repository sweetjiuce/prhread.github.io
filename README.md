## Welcome to GitHub Pages
## Welcome to GitHub Pages
### namespace 详解
namespace 中文解释为命名空间
为什么要有这个命名空间呢？为了区分班上同名的同学。一个文件夹不能创建同名同种类型的文件，但是一个文件夹里的多个文件夹里可能有多个重名的文件。
命名空间的存在就是为了避免不同的库中不同的函数名称一样，从而导致系统在编译时 不知道是哪一个库的函数名称。

### C++ inline 关键字

inline的引用是为了解决在使用过程中 频繁的调用函数 从而导致程序的栈空间被消耗枯竭的问题，inline 表示为内联函数
实例
#include <stdio.h>
//函数定义为inline即:内联函数
```
inline char* dbtest(int a) {
    return (i % 2 > 0) ? "奇" : "偶";
} 
 
int main()
{
   int i = 0;
   for (i=1; i < 100; i++) {
       printf("i:%d    奇偶性:%s /n", i, dbtest(i));    
   }
}
