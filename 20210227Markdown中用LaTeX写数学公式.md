# Markdown中用LaTeX写数学公式

环境：在Typora用Markdown写LaTeX，注意打开下面的偏好设置：

![image-20210227181715493](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227185335.png)

## 插入公式

- Inline mode（行间公式）

  这是一个行间公式  $y = x^2$

- Display mode（独立公式）


$$
y = x^2
$$



## 基础语法

| 说明 | LaTex | 输出                           |
| ----- | ----- | ---------- |
| **上下标** |  |  |
| 上标 | a^2 | $a^2$  |
| 下标   | a_2 |        $a_2$                        |
| 复杂上下标 | a^{2+2} | $a^{2+2}$ |
| 上下标组合 | a_2^3   | $a_2^3$ |
| 导数 | x' |    $x'$    |
|  |  |  |
| **分式和根式** |  |  |
| 分式 | \frac{a}{b} | $\frac{1}{a}$ |
| 连续分式 | \cfrac{1}{a + \cfrac{1}b} | $\cfrac{1}{a + \cfrac{1}b}$ |
| 根式 | \sqrt[n]{x} | $\sqrt[n]{x}$ |
|  |  |  |
| **关系符与运算符** |  |  |
| 直接可输入的 | \+ - = ! / () [] <> \| ' : * | $+ - = ! / () [] <> | ' : *  $ |
| 不等号 | \ne | $\ne$ |
| 大于等于号 | \ge | $\ge$ |
| 小于等于号 | \le | $\le$ |
| 约等号 | \approx | $\approx$ |
| 等价 | \equiv | $\equiv$ |
| 乘号 | \times | $\times$ |
| 除号 | \div | $\div$ |
| 点乘 | \cdot | $\cdot$ |
| 加减号 | \pm | $\pm$ |
| 三角函数 | \sin(a)   \cos(a) | $\sin(a)$ |
| 求和号 | \int | $\int$ |
| 积分号 | \sum | $\sum$ |
| 极限 | \lim | $\lim$ |
| 对数log | \log | $\log$ |
| 对数lg | \lg | $\lg$ |
| 对数ln | \ln | $\ln$ |
|  |  |  |
| **特殊符号** |  |  |
| 省略号 | \dots | $\dots$ |
| 右箭头 | \rightarrow 或 \to | $\rightarrow$ |
| 左箭头 | \leftarrow 或 \gets | $\leftarrow$ |
| 花括号 | `\{a\}` | $\{a\}$ |
| 插入文字 | \text{apple} | $\text{apple}$ |
| 空格 | \quad | $(\quad)$ |


其他：

- 希腊字母

  ![在这里插入图片描述](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227185336.JPG)



## 举个栗子

- 二元一次方程 + 求根公式

  二元一次方程：
  $$
  y = a\cdot x^2 + b\cdot x + c
  $$
  

  y=0时，求根公式：
  $$
  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
  $$
  
- 宏观经济学中的泰勒公式
  $$
  \begin{aligned}
  &\text{Target nominal short-tem interest rate}\\
  & = (r_{real} + i_{target}) + 0.5(GDP_{expect} + GDP_{target}) + 0.5(i_{expect} - i_{target})
  \end{aligned}
  $$
  



## 参考链接

- [如何在1小时内快速入手LaTeX](https://www.zhihu.com/question/268569440)
- [Typora中利用LaTeX 插入数学公式](https://blog.csdn.net/happyday_d/article/details/83715440)
- [LaTeX/Mathematics](https://en.wikibooks.org/wiki/LaTeX/Mathematics)