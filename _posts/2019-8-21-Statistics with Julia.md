---
layout: post
title: 《使用 Julia 语言学习统计学》
categories: Julia
---

**Julia** 是一个面向科学计算的高性能动态高级程序设计语言。其语法与其他科学计算语言相似。在许多情况下拥有能与编译型语言相媲美的性能。Julia 是个灵活的动态语言，适合科学和数值计算，性能可与传统静态类型语言媲美。

> 免费英文电子书，大学本科的统计学入门教材，其中的示例使用简单的 Julia 语言。[《使用 Julia 语言学习统计学》](https://people.smp.uq.edu.au/YoniNazarathy/julia-stats/StatisticsWithJulia.pdf)

### **Introducing Julia**

Programming goes hand in hand with mathematics, statistics, data science and many other fields. Scientists, engineers, data scientists and statisticians often need to automate computation that would otherwise take too long or be infeasible to carry out. This is for the purpose of prediction, planning, analysis, design, control, visualization or as an aid for theoretical research. Often, general programming languages such as Fortran, C/C++, Java, Swift, C#, Go, JavaScript or Python are used. In other cases, more mathematical/statistical programming languages such as Mathematica, Matlab/Octave, R, or Maple are employed. The process typically involves analyzing the problem at hand, writing code, analyzing behavior and output, re-factoring, iterating and improving the model. At the end of the day, a critical component is speed, specififically, the speed it takes to reach a solution - whatever it may be.

![1566355025068](..\images\1566355025068.png)

The *Julia language and framework* developed in the last several years makes use of a variety of advances in compilation, computer languages, scientifific computation and performance optimization. It is a language designed with a view of improving on the previous Pareto-optimal frontier depicted in Figure 1.1. With syntax and style somewhat similar to R, Python and Matlab/Octave, and with performance comparable to that of C/C++ and Fortran, Julia attempts to break the so called *two* *language problem*. That is, it is postulated that practitioners may quickly create code in Julia, which also runs quickly. Further, re-factoring, improving, iterating and optimizing code can be done in Julia, and does not require the code to be ported to C/C++ or Fortran, since the Julia standard libraries, and almost all of Julia base are written in Julia.

...

> 本书代码库 地址：
>
> [https://github.com/h-Klok/StatsWithJuliaBook](https://github.com/h-Klok/StatsWithJuliaBook)




Julia is first and foremost a *scientific programming language*. It is perfectly suited for statistics, machine learning, data science and for heavy (as well as light weight) numerical computations. It can also be integrated in user-level applications, however one would not typically use it for front-end interfaces, or game creation. It is an open-source language and platform, visit [https://julialang.org/](https://julialang.org/) for more details. The Julia community brings together contributors from both the scientific computing world and the statistics and data-science world. This puts the Julia language and package system in a good place for combining mainstream statistical methods with methods and trends of the scientific computing world. Coupled with programmatic simplicity similar to Python, and with speed similar to C, Julia is taking an active part of the data-science revolution. In fact, some believe it will become the primary language of data-science in the future.

(at the moment, most people believe that Python holds this title). 

...

#### Julia简单的例子

```julia
1 println("There is more than one way to say hello:") 
2
3 #This is an array consisting of three strings 
4 helloArray = ["Hello","G’day","Shalom"] 
5
6 for i in 1:3 
7 println("\t", helloArray[i], " World!") 
8 end 
9 
10 println("\nThese squares are just perfect:") 
11 
12 #This construct is called a ‘comprehension’ (or ’list comprehension’) 
13 squares = [i^2 for i in 0:10] 
14 
15 #You can loop on elements of arrays without having to use indexing 
16 for s in squares 
17 print(" ",s) 
18 end
19 
20 #The last line of every code snippet is also evaluated as output (in addition to 
21 # any figures and printing output generated previously). 
22 sqrt.(squares) 
```
##### 输出结果  

There is more than one way to say hello:  
	Hello World!  
	G’day World!  
	Shalom World!  
These squares are just perfect:   
0  1  4  9  16  25  36 49  64  81  100  
11-element Array{Float64,1}:  
0.0  
1.0  
2.0  
3.0  
4.0  
5.0  
6.0  
7.0  
8.0  
9.0  
10.0  

#####  Julia的运行
1.[**Julia’s REPL interface**](https://julialang.org/downloads/)
![1566358084728](..\images\1566358084728.png)

>[Julia官方语言的文档](https://docs.julialang.org) 


2. [**JuliaBox**](https://juliabox.com/):一个无需下载安装任何东西，使用浏览器即可在 **Jupyter Notebook** 中直接运行 **Julia** 代码的平台。


