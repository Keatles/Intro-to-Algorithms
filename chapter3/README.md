## 第三章 函数的增长

### 基本概念

![](3-1-1.gif)

![](3-1-2.gif)

## 练习

### 3.1-1假设f(n)和g(n)都是渐进非负函数。使用θ记号的基本定义来证明max(f(n),g(n))=θ(f(n)+g(n))

因为max(f(n),g(n))<=f(n)+g(n),所以存在c=1,n<sub>0</sub>=1,任意的n>=n<sub>0</sub>,max(f(n),g(n))<=c(f(n)+g(n)

又因为max(f(n),g(n))>=1/2(f(n)+g(n)),所以存在c=1/2,n<sub>0</sub>=1,任意的n>=n<sub>0</sub>,max(f(n),g(n))>=c(f(n)+g(n))

### 3.1-2 证明:对任意实常量a和b,其中b>0，有(n+a)<sup>b</sup>=θ(n<sup>b</sup>)

![](3-1-3.gif)

### 3.1-3 解释为什么"算法A的运行时间至少是O(n<sup>2</sup>)"这一表述是无意义的。

算法A的运行时间至少是b，则表示算法A运行时间>=b,因为b=O(n^2),并且f(n)=c=O(n^2),因此这句话表示**算法A的运行时间可以是任何值**。 

### 3.1-4 2<sup>n+1</sup>=O(2<sup>n</sup>)成立吗?2<sup>2n</sup> = O(2<sup>n</sup>)成立吗?

2<sup>n+1</sup> = O(2<sup>n</sup>)，2<sup>2n</sup> != O(2<sup>n</sup>)

为了证明2<sup>n+1</sup> = O(2<sup>n</sup>),必须找到常量c,n<sub>0</sub>>0让n>=n<sub>0</sub>情况都满足0<=2<sup>n+1</sup><=c.2<sup>n</sup>

可以找到c=2和n<sub>0</sub>=1时对所有n都满足2<sup>n+1</sup> = 2*2<sup>n</sup>

为了证明2<sup>2n</sup> != O(2<sup>n</sup>),假设存在常量c,n<sub>0</sub>>0在所有n>=n<sub>0</sub>的情况下都满足0<=2<sup>2n</sup><=c·2<sup>n</sup>

则2<sup>2n</sup> = 2<sup>n</sup>·2<sup>n</sup><=c·2<sup>n</sup> 即2<sup>n</sup><=c 但没有常量比2<sup>n</sup>大所以假设是不成立的。



### 证明定理3.1

![](3.1-5.gif)

### 证明:一个算法的运行时间为θ（g(n))当且仅当其最坏情况运行时间为O(g(n)),且其最好情况运行时间为Ω(g(n))

![](3.1-6.gif)

### 证明:o(g(n))∩ω(g(n))为空集

![](3.1-7.gif)

