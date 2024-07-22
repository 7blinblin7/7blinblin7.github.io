---
layout: post
title:  "Java L4"
date:   2024-07-22 14:41:08 +0800
categories: jekyll update
---
#1.接口
1. 包含未定义方法 不能使用new实例化 可以声明  没有构造函数

2. 所有变量是public final 所有方法是public abstract 所以public可以省略 接口中常量可以通过interfacename.constant_name来访问  

3. 抽象方法使用场景 当类无法清楚定义方法内容可以使用抽象方法  
接口使用实例```java  

class Apple implements Colorable {
@Override
public void color() {
System.out.println(“Red");
}
}  

class Banana implements Colorable {
@Override
public void color() {
System.out.println(“Yellow");
}
}  

public interface Colorable {
abstract public void color();
}
InterfaceDemo```  
#2.抽象类
1. 抽象类可以有抽象和非抽象方法 含有抽象方法必须是抽象类 同接口一样只能声明不能实例化 但是有构造函数 通过构造函数列进行调用
2. 如果抽象超类的子类没有实现/覆盖所有抽象方法，则该子类将继承抽象方法，并且必须声明为抽象
3. 它的抽象方法强制其子类提供实现。Java 语言不允许实例化抽象类型并强制子类型实现所有需要的功能，这一事实进一步确保了程序的正确性。
#3.多重继承   
1. 所有类共享一个根，即 Object 类，但接口没有单个根
2. 接口可以多重继承 类只能单一继承 类可以实现多个接口
#4.面向对象流程
需求分析 系统分析 系统设计 实现 测试 部署 维护
#5.crc
类相似对象 责任 类知道做的事 协作者 需要交互的其他类
#6.耦合
低耦合高内聚 系统更稳定 耦合程度由低到高：关联、聚合、组合、实现和泛化  

1. 关联 学生和老师同时因为课程而关联 通过数据字段实现
2. 聚合和组合表示整体和部分的关系 has a 组合比聚合更强因为 组合代表随着父类的消失子磊也会消失 has a关系 实心菱形(组合)和空心菱形（聚合）
3. 普遍化和实现 is a extends 和 is kind of a implements实现箭头和虚线箭头
4. 关心多态则使用继承不关心多态则使用聚合更加灵活
#7.内部类
1. 成员内部类
2. 局部内部类
3. 匿名内部类




