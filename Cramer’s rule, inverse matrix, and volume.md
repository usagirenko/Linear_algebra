- Solving linear equations
- Computing the inverse matrix

## Solving $Ax=b$ by Cramer's rule

- $\begin{bmatrix}a_{11} & a_{12} & a_{13}\\ a_{21} &a_{22} & a_{23}\\ a_{31} &a_{32} &a_{33}\end{bmatrix}\begin{bmatrix}x_{1}\\x_{2}\\x_{3}\end{bmatrix}=\begin{bmatrix}b_{1}\\b_{2}\\b_{3}\end{bmatrix}$

## Multiply A by X1
- $$
\begin{bmatrix}a_{11} & a_{12} & a_{13}\\ a_{21} &a_{22} & a_{23}\\ a_{31} &a_{32} &a_{33}\end{bmatrix}\begin{bmatrix}x_{1} & 0 & 0\\ x_{2} &1 & 0\\ x_{3} &0 &1\end{bmatrix}=\begin{bmatrix}b_{1} & a_{12} & a_{13}\\ b_{2} &a_{22} & a_{23}\\ b_{3} &a_{32} &a_{33}\end{bmatrix}
$$
$$
A\qquad \qquad \qquad  X_{1}\qquad \qquad B_{1}
$$

$$
\det(AX_{1})=\det(A)\det(X_{1})=\det(B_{1})
$$
$\det(A)x_{1}=\det(B_{1})$
$x_{1}=\frac{\det(B_{1})}{\det(A)}$
$x_{2}=\frac{\det(B_{2})}{\det(A)}$
$x_{3}=\frac{\det(B_{3})}{\det(A)}$


## Formula for $A^{-1}$

![[Pasted image 20241210151511.png]]
multiply both side by A:
$$
I(\det A)= AC^T
$$
![[Pasted image 20241210152749.png]]

## use the determinant to calculate area/volume,cross product and so on

the geometric meaning of the $A\times B$ is the area of the parallelepiped.
just like the determinant
so  
$$
a\times b=\det
\begin{bmatrix}
i & j & k \\
a_{x} & a_{y} & a_{z} \\
b_{x} &b_{y} & b_{z}
\end{bmatrix}=
$$
 ![[Pasted image 20241210160526.png]]
![[Pasted image 20241210160128.png]]
## volume($(A\times B)\cdot C$)
![[Pasted image 20241210160856.png]]
### Much easier 

***just*** $\det \begin{bmatrix}a & b &c\end{bmatrix}$