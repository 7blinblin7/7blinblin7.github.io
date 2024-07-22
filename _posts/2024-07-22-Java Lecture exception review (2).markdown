---
layout: post
title:  "Java L6"
date:   2024-07-22 14:41:08 +0800
categories: jekyll update
---
#1.异常
1. checked 异常 编译时异常 unchecked 异常 runtime and error
2. 顺序 声明 抛出 捕获异常 转发异常 throw ex；
3. try catch finally语句及其执行顺序 如果转发则不执行其他catch
4. try with resource 优势 简单处理
5. 优点：与代码分开 向上传播
#2.断言  
1. 不用于处理错误 会直接推出
2. 常用做法 将注释中判断条件改为断言
3. 区别：
异常处理处理程序执行期间的异常和意外情况，并提供从错误中恢复的机制。断言用于确保整个程序执行过程中的（正确）条件。
异常解决稳健性（从错误中恢复），断言解决正确性（确认没有错误）。



