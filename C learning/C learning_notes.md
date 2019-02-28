# C learning notes

## Content
- [推荐教程/教材](#textbook)
- [学习笔记](#notes)
	- [知识点](#Keypoints)	
- [Code Commands](#Code_Commands)




## <h1 id="textbook">推荐教程/教材</h1>

教程名称 | 参考书 | Notes等其他资料 | 学习状态  
:-- | :--: | :--: | :--: 
C语言开发从入门到精通(书)| 此书||学习中
C Primer Plus | 此书 | |学习中
C和指针 | 此书





## <h1 id="notes"> 学习笔记 </h1>


#### <h2 id="flow_control"> - 流程控制语句 </h2>


**break** 
>  break语句通常用在循环语句和开关语句中。当break用于开关语句switch中时，可以使程序跳出switch而执行switch以后的语句；如果没有break语句，则将成为一个死循环而无法退出。

break语句的功能如下所示：
>
- 改变程序的控制流。
- 用于do-while、while、for循环中时，可使程序终止循环而执行循环后面的语句。
- 通常在循环中与条件语句一起使用，若条件值为真则跳出循环，控制流转向循环后面的语句。
- 如果已执行break语句，就不会执行循环体中位于break语句后的语句。
- 在多层循环中，一个break语句只向外跳一层。

**continue** 
> continue语句的功能是，跳过循环体中剩余的语句而强行执行下一次循环。continue语句只用在for、while、do-while等循环体中，常与if条件语句一起使用，用来加速循环。

continue语句的功能如下所示：
>
- continue语句只能用在循环里。
- continue语句的作用是跳过循环体中剩余的语句而执行下一次循环。
- 对于while和do-while循环，continue语句执行之后的动作是条件判断；对于for循环，随后的动作是变量更新。

**退出程序 exit()**
> 在C语言项目中，程序执行到main函数右边的花括号“}”后，程序将结束。实际上，在main函数结束时，会隐式地调用退出函数exit。

```
void exit(int status);
```
> 其中，“status”表示退出状态，一般用0表示正常退出，如果是非0则表示不退出。

```
#include < iostream> 
#include < string> 
using namespace std; 
int main() { 
　exit (1);　　　　　　　//等价于return (1); 
}

```

#### <h2 id="pointer" > - Pointer</h2>

在C语言中，有如下两个和指针变量有关的元素。

（1）&：取地址运算符

```
&变量名；
```

（2）*：指针运算符（或称“间接访问” 运算符）

```
存储类型 数据类型 *指针变量名1[=初值1]；

```





## <h1 id="Code_Commands"> Code Commands </h1>

