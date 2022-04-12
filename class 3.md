CG中经常把效果夸大，做的plausible和exaggerated

## 碰撞检测
问题：
1. 哪些三角形和地面相交
2. 哪些点在地面下面哪些在上面

penalty force，计算点和平面之间的距离，✖️上一个系数。

判定点是否在任意平面下面：
1. 计算法向量，判断和法向量的夹角是钝角还是锐角
2. 计算Ax+By+Cz+d是否大于0

## Solving Linear Systems
### Linear Systems
$Ax=b$ A is a matrix and x is a vector and b is another vector.

- Small (maby up to 200\*200)
	- Symmetric? ($A = A^T$)
		- Modified Cholesky $A = PLDL^T$
	- not Symmetric
		- Gaussian Elimination $A=PLU$
	- Matlab
	- gnu octave
	- Blas/ Lapack(C++ library)
	- Intel Math Kernel Library(MKL)
	- Eigen
- Large
	- Sparse
		- Symmetric
			- Sparse cholesky
			- Conjugate iterative
			- Gradients iterative
			- Pardiso
			- Taucs
			- Mumps 
		- not Symmetric
			- Sparse LU
	- not Sparse
		- 复杂度为$O(n^3)$