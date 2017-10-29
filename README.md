# SVM_py
svm理论学习与实现
* svm理论基础要点概括
  * 如何理解核函数？
  * 拉格朗日乘子法的作用？
  
  
  
  
* 如何理解核函数？
Let κ be a kernel function on ℝd×ℝd- a function such that the matrix K with Kij=κ(xi,xj) is positive semidefinite. A key property of such kernel functions is that there exists a map ν such that ⟨ν(x),ν(y)⟩=κ(x,y). One can think of ν as mapping our input features into a higher dimensional output space.
这一段翻译起来为：核函数K是一个函数，能够将输入特征映射到更高的空间中。看过一个比较好的解释，如果输入特征X为x1,x2。则X与y之间线性可预测时的公式为ax1+bx2=y。当线性不可分时，对输入特征作变换，X的特征为x1*x1,x2*x2,x1*x2。这时将特征拓展到3维空间，恰好可分即存在一个分类平面。而这时特征恰好是向量点积的结果。所以可以定义核函数K=（x1,x2)*(x1,x2).所以将复杂的向高维映射可以简单的定义为向量之间的点积。

* 拉格朗日乘子法的作用？
将约束条件加入到问题求解中。一个例子就是隨球内求最大体积的长方体。
