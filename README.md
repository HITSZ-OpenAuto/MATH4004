# MATH4004 - 数值分析

![考查课](https://img.shields.io/badge/%E8%80%83%E6%9F%A5%E8%AF%BE-green)
![学分](https://img.shields.io/badge/%E5%AD%A6%E5%88%86-2-moccasin)
![研究生阶段跨选](https://img.shields.io/badge/研究生阶段跨选-lightskyblue)

![成绩构成](https://img.shields.io/badge/%E6%88%90%E7%BB%A9%E6%9E%84%E6%88%90-gold)
![出勤10%](https://img.shields.io/badge/出勤-10%25-wheat)
![课堂测验及作业20%](https://img.shields.io/badge/课堂测验及作业-20%25-wheat)
![期末考试70%](https://img.shields.io/badge/%E6%9C%9F%E6%9C%AB%E8%80%83%E8%AF%95-70%25-wheat)

目前研究生阶段课程资料甚少，敬请各位贡献。教材与参考书见校内网盘（资料下载部分）。

## 教材及参考书

- 李庆扬等，数值分析（第五版）。
- 并非每一章都包含在教学内容中，具体内容见校内网课件。

## 课程内容

{{% details title="第一章 绪论" closed="true" %}}
主要内容是：课程特点、线性代数基础知识、泰勒（Taylor）公式、收敛阶数等。
{{% /details %}}

{{% details title="第二章 计算机算术" closed="true" %}}
主要内容是：浮点数和舍入误差，绝对误差和相对误差，计算的稳定性。
{{% /details %}}

{{% details title="第三章 线性方程组的求解" closed="true" %}}
主要内容是：线性方程组的直接求解和迭代求解。直接求解部分，主要讲解了 Gauss 消元法、LU 分解（及其变种 Crout 分解）、Cholesky 分解、列主元 Gauss 消元法等。迭代求解部分，补充了矩阵范数的相关知识，依次介绍了 Jacobi 迭代法、Gauss-Seidel 迭代法和逐次松弛（successive over relaxation，简称 SOR）迭代法。重点在于各迭代法的收敛性分析。前两种迭代法的公式需要会自行导出，最后一种了解参数$omega$的意义即可。
{{% /details %}}

{{% details title="第四章 函数逼近与计算" closed="true" %}}
主要内容是：插值和拟合。所讲解的插值方法包括拉格朗日（Lagrange）插值、牛顿（Newton）插值、埃尔米特（Hermite）插值以及相应的分段插值方法。重点是各种插值方法的误差分析。所讲解的拟合方法为最小二乘拟合（以及广义最小二乘拟合），包括对函数的拟合与对离散点的拟合（都要熟练掌握），涉及正交多项式等概念。
{{% /details %}}

{{% details title="第五章 数值微分与数值积分" closed="true" %}}
主要内容如题。数值微分部分，讲解了基于插值方法得到的求导公式，以及充分利用泰勒展开式得到的理查德森（Richardson）外推法。数值积分部分，讲解了对应于插值方法的积分公式，对应于分段插值的复合求积，对应于理查德外推法的龙贝格（Romberg）积分，以及优化节点从而得到更高精度的高斯求积（Gauss Quadrature）。本章的重难点在于理解代数精度的概念以及掌握提高代数精度的方法，各种求积公式的形式与构造也是很重要的。
{{% /details %}}

{{% details title="第六章 常微分方程的数值解法" closed="true" %}}
主要内容是：重点介绍单步法，也介绍了多步法。单步法包括欧拉法、梯形法、改进的欧拉法和龙格库塔（Runge-Kutta）法。本章的重点概念是局部截断误差和精度阶数，需要熟练掌握。需要理解龙格库塔法的基本思想，至于其基于多元函数泰勒展开式的繁琐推导，可作为闲暇时刻的消遣。
{{% /details %}}

{{% details title="第七章 非线性方程的求解" closed="true" %}}
主要内容是：迭代求解方法，如二分法、牛顿法和弦截法。具体方法原理易懂，操作简单。对于一般的迭代法，需要掌握简单情形下的收敛性分析。对于二分法、牛顿法和弦截法这三种方法，需要掌握其原理、收敛性分析和误差分析。
{{% /details %}}

> 文 / [Oliver Wu](https://github.com/OliverWu515) 与 [Hye](https://github.com/Co-ding-Man), 2025.1.4

## 授课教师

本研共选课（面向保研学生开设，一般开设于秋季学期 10-17 周）：

- 焦震钧
  - 每节课前会回顾上节课的内容。
  - 每章课件会在上本章之前发放，不过有可能不是最新版本——课上还会出现新的插图（不过基本内容不变）。
  - 松弛感满满，很擅长举简明的例子帮助学生理解，颇有“四两拨千斤”的感觉。举几个上课过程中印象深刻的点：从 $2 x = 1$ 的迭代求解引出复杂线性方程组的迭代求解；插值基函数的讲解；以平均数讲解生活中的最小二乘（使用零次多项式，即常数，进行最小二乘近似）。
  - 不过，有些较高观点的理解较为抽象，可能需要比较好的空间想象力和线性代数基础才能听懂。

> 文 / [Oliver Wu](https://github.com/OliverWu515) 与 [Hye](https://github.com/Co-ding-Man), 2025.1.4 

研究生课（面向研一学生开设，一般开设于秋季学期 1-8 周）：

- 张茜

## 关于考试

数值分析本来就是面向计算机运算的科学，所以许多算法并不适合用于手工计算，考试也不会堆计算量恶心人。考前最后一节课老师会给大家梳理重点，建议认真听。课件例题、作业题、往年题都很经典，建议认真看，考试可能有类似的问题。

> 文 / [Oliver Wu](https://github.com/OliverWu515), 2025.1.4

## 学习建议

感受每种数值算法背后蕴涵的严谨/直观的数学思想（比如，外推法是如何提高精度的？Gauss 求积公式为何能实现更高的代数精度？谱半径、范数衡量的是矩阵的何种特征？），比会手动算出（本来就是给计算机用的）数值积分更为有益。

> 文 / [Oliver Wu](https://github.com/OliverWu515), 2025.1.4
