# CPP-King
我要精通C++
tips:代码开发出来是要实际应用的，学习相关C++现代特性时，多思考实际工程应用
1.C++是工程语言，往往有大量技术人员一起开发，不可避免的出现命名重复的问题，因此需要有namespace
## C++代码编写规范
---
## 一些C++前置:
1. ::作用域运算符(在ros系统开发中经常用到)
相关:生命周期，全局变量，局部变量，命名空间，static，类
tips:
命名空间只能全局命名；命名空间是开放的；命名空间内的函数可以访问空间内的变量，这是全局变量
```cpp
namespace LongName{
}
// 取别名，实际上是复制给ShortName
int main(){
  namespace ShortName = LongName;
}
```
```cpp
namespace A{
  int a;
}
namespace A{
  void func(){}
}
```
```cpp
#include <iostream>
int a =10;
int main()
{
  std::cout<<a<<endl;
  std::cout<<::a<<endl;
}
```
3.
# 第一部分:面向对象
### 构造函数集合:
一般使用构造函数与拷贝构造函数 
### 内联函数

# 第二部分:泛型编程
