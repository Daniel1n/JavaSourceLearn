# JavaSourceLearn
观看B站up主CodeSheep
<br> 《Java源码盘起来！演示搭建JDK源码阅读环境，利用IDEA搭建Java源码阅读环境视频教程》
<br> 学习如何搭建JDK源码的阅读环境

前面的步骤都没问题，唯独发现两个问题

1.报的错误是与tools包相关的缺失问题
- java:程序包com.sum.tools.javac.api不存在
- java:程序包com.sun.tools.javac.processing不存在
- java:程序包com.sun.tools.javac.util不存在

解决办法：在Project Structure中的Libraries添加tool.jar（来源是jdk的lib）

2.报错UNIXToolkit类和FontConfigManager
- 解决办法：直接把报错的包com.sun.java.swing.plaf.删除
