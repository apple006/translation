# 1. 基本数据类型

Java归纳了8种基本数据类型:

int, 整数型, 32位, 2^32; 约 +-40E/2 = 20亿;
long, 长整型, 64位, 2^64; 
float, 32位浮点型, 也叫单精度;
double, 双精度, 64位浮点型; 浮点的意思是小数点是浮动的。不固定整数占多少位, 不固定小数占多少位;
byte, 字节, 1字节=8bit=8位;
short, 短整型, 16位;
char, 字符型, 16位Unicode表示。
boolean, 布尔值, 只有真假/true/false; 对应二进制就是1/0;

初始化时会所有bit位填零(0/1)；

当然, 对应的都有包装类型。

自动装包,拆包基本类型, 是在编译时转换为 Integer.valueOf(); 以及 Integer#intValue(); 等方法进行实现的。 参考 .class 文件反编译之后的代码即可。 推荐 jd-gui 工具。


# String类型

字符串, 本质是一个一个的字符。 再究其本质, 涉及到编码, 在计算机中就是一个一个的字节排列成为字节流, 再涉及到大端字节序, 小端字节序, 那本质就是一串串的bit;二进制位。 按照规定排列, 存储, 传输, 读取即可。

因为Java的 String 对象不允许进行修改, 虽然底层使用 chat[] 来存储, 却可以认为是一维数据; 一切都是为了有组织, 人类/程序员阅读和使用方便。

所以,数据结构, 就是将数据(data, bit, byte, 一维数据)组织起来, 打包成为一个整体, 以方便使用和理解。

所以, 数据结构的本质就是封装。 当然, 因为一维数据是基础, 而且相对比较简单, 所以很多书籍不将他们作为数据结构进行讲解。

面向对象的封装, 可以分为多个角度来看, 比如, 数据封装, 逻辑封装, 代码组织形式的封装等等。 参考快递包裹的打包和封装。




