---


Title: 线性方程组
Author: Desnity
Date: 2018.12.13
---

# 线性方程组

[TOC]



## 解的判定

线性方程组有解的充要条件是它的系数矩阵的秩等于增广矩阵的秩。

即$Ax=\beta$ 有解的充要条件为 $R(A) = R((A|\beta))$



对于n元线性方程组

- 当$R(A)=R((A|\beta)) = n$ 时有唯一解
- 当$R(A)=R((A|\beta)) = r < n$时有无穷多个解，且通解中包含 n-r 个任意参数



特别的，对于n元齐次线性方程组$Ax=0$

- 当$R(A)= n$ 时只有零解
- 当$R(A) = r < n$时有无穷多个解，且通解中包含 n-r 个任意参数



## 解的结构

### 齐次线性方程组

**齐次线性方程组解的性质** 

- 设$\xi_{1},\xi_{2}$ 是齐次线性方程组$Ax=0$ 的两个解向量，则$\xi_{1} + \xi_{2}$ 也是齐次线性方程组$Ax=0$ 的解向量。
- 设$\xi$ 是齐次线性方程组$Ax=0$ 的两个解向量，k是任意常数，则$k\xi$ 也是齐次线性方程组$Ax=0$ 的解向量。

*即：解向量的集合对解向量的线性运算是封闭的*



**基础解系**

定义：

设$\xi_{1},\xi_{2},···,\xi{s}$ 是齐次线性方程组$Ax=0$ 的一组解向量，若满足

1. $\xi_{1},\xi_{2},···,\xi{s}$ 线性无关
2. $Ax=0$ 的任意解都可由$\xi_{1},\xi_{2},···,\xi{s}$ 线性表出

那么$\xi_{1},\xi_{2},···,\xi{s}$ 称为齐次线性方程组$Ax=0$的一个基础解系。



对于n元齐次线性方程组$Ax=0$，若$R(A) = r < n$，则基础解系含有n-r个向量



### 非齐次线性方程组

**导出组**

将$Ax=0$称为$Ax=\beta$ 的导出组。



**非齐次线性方程组解的性质**

- 非齐次线性方程组的任意两个解的差是它的导出组的解
  - 若$\eta_{1},\eta_{2}$都是$Ax=\beta$ 的解，则有$A\eta_{1}=\beta$,$A\eta_{2}=\beta$,所以$A(\eta_{1}-\eta_{2})=0$
- 非齐次线性方程组的一个解$\eta$ 与其导出组的一个解$\xi$ 之和仍是该非齐次线性方程组的一个解
  - 因为$A\eta = \beta,A\xi = 0$ ，所以$A(\eta + \xi) = \beta + 0 = \beta$
- $\eta_{0}$ 为非齐次线性方程组的某个解，$\xi$ 是其导出组的一个解，则该非齐次线性方程组的任意解都可以表示为$\eta_{0} + \xi$



**解的结构**

则通解可以表示为一个特解加上导出组解的线性组合。

