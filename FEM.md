# Finite Element Method
Triangle mesh is embedded in the 3 dimensional solid mesh

FEM can solve any partial differential equations. Here we solve elasticity for 3D solid.

Deformation Gradient: 如果已知一个点变形后的位置，想知道它附近的点变形后的位置
就是三维插值方程。

核心思路是不solve for continuous, 算出三角形顶点的结果然后做插值

FEM shape function, consistent Mass. We use lumped mass in HW1

![[Pasted image 20220507010040.png]]
![[Pasted image 20220507011501.png]]

![[Pasted image 20220507020932.png]]
FEM is not popular when it just invented, because there is no computer back then.

Use gauss point to do the numerical approximation of integral for 3D

## Linear and Co-rotational FEM
Linear FEM model:
- wrong on large deformation
- precise on small deformation
- fast computation
- used in 建筑行业

Co-rotational FEM model:
- 用旋转后的结果来模拟最终结果
- 先算出deformation gradient然后用polar decomposition将其分解成rotation和一个对称矩阵
- works well when there's small deformation on top of rotation

![[Pasted image 20220507032730.png]]