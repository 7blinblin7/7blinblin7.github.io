---
layout: post
title:  "Java L5"
date:   2024-07-22 14:41:08 +0800
categories: jekyll update
---
#1.泛型  
1. 泛型通过在编译时可检测到更多错误来增加代码的稳定性。example:  
``` Box<Integer> integerBox = new Box<Integer>();
```
2. 类型安全且更易于阅读 不需要强制转换
3. 类型约定 大写字母 约定如下：E元素K键N数字T类型V值SUV第二三四个值
4. 钻石<>
在 Java SE 7 及更高版本中，只要编译器可以从上下文中确定或推断类型参数，就可以将调用泛型类构造函数所需的类型参数替换为一组空的类型参数 （<>）。  
```Box<Integer> integerBox = new Box<>();
```
#2. 通用方法
1. 类型推断 编译器将推断所需类型 允许将泛型方法像普通方法一样调用
2. 有界类型  您可能希望限制可用作参数化类型中的类型参数的类型  
```public <U extends Number> void inspect(U u)```
3. 泛型类型调用 ```Box<Number> box = new<>Box(); box.add(new Integer(10));```is ok 因为integer是number的子类  
```public void boxTest（Box<Number> n） { /* ... */ }```不可以接受Box<Integer> 和 Box<Double> 因为Box<Integer> 和 Box<Double> 不是 Box 的子类型<Number>。
#3. 通配符  
1. 用于泛型类型的实例化和方法参数。
2. 有界通配符 ？ extends B 上界? super B下界
#4. JCF  
1. C++ 标准模板库 （STL） 的 Java 对应物
2. 接口算法实现



