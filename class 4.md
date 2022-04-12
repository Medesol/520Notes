常用的库：
- Intel TBB,并行计算
- Intel MKL,线性代数
- MMX/SSE/AVX, 乘法
- boost，load and reload
- cuda
- Pthreads
- Openmp
- Eigen, wrapper for MKL 

Solving system of equations:
- Newton-Raphson method
 
Timestepping ODEs：
- Euler's Method（Forward order） $y_{n+1}=y_n+hG(y_n)$ ,如果h比较大，会慢慢blowup
- Backward Euler's Method $y_n=y_{n+1}-hG(y_n)$
	- $hG(y_n)=[I-hG_\prime(y_n)]\Delta y_n$左边已知，右边线性