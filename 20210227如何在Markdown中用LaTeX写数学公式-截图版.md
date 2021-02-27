# 如何在Markdown中用LaTeX写数学公式

环境：在Typora用Markdown写LaTeX，注意打开下面的偏好设置：

![image-20210227181715493](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227185335.png)

## Markdown中插入LaTeX公式

- Inline mode（行间公式）

  这是一个行间公式  $y = x^2$

- Display mode（独立公式）


$$
y = x^2
$$



## LaTeX基础语法

![image-20210227185926673](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227190955.png)

![image-20210227185944967](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227190956.png)

![image-20210227190219314](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227193157.png)

![image-20210227190007389](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227190957.png)



其他：

- 希腊字母

  ![在这里插入图片描述](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227185336.JPG)



## 举个栗子

- 二元一次方程 + 求根公式

  二元一次方程：
  $$
  y = a\cdot x^2 + b\cdot x + c
  $$
  
![image-20210227190048577](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227190959.png)
  
  y=0时，求根公式：
  $$
  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
  $$
  ![image-20210227190219314](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227193229.png)
  
- 宏观经济学中的泰勒公式：

  ```latex
  $$
  \begin{aligned}
  &\text{Target nominal short-tem interest rate}\\
  & = (r_{real} + i_{target}) + 0.5(GDP_{expect} + GDP_{target}) + 0.5(i_{expect} - i_{target})
  \end{aligned}
  $$
  ```

![image-20210227190202122](https://raw.githubusercontent.com/Hawking8su/Images/main/20210227191001.png)

## 参考链接

- [如何在1小时内快速入手LaTeX](https://www.zhihu.com/question/268569440)
- [Typora中利用LaTeX 插入数学公式](https://blog.csdn.net/happyday_d/article/details/83715440)
- [LaTeX/Mathematics](https://en.wikibooks.org/wiki/LaTeX/Mathematics)