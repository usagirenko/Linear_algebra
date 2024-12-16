>The determinant of a matrix is a single number which encodes a lot of information about the matrix. Three simple properties completely describe the determinant. In this lecture we also list seven more properties like detAB = (detA)(detB) that can be derived from the first three.

## Properties

We already know that $\begin{bmatrix}a & b\\ c & d\end{bmatrix}=ad-bc$.These properties will give us a c d formula for the determinant of square matrices of all sizes.
1. $\det I=1$
2. If you exchange two rows of a matrix, you ***reverse the sign*** of its determinant from positive to negative or from negative to positive.
3.  (a) If we multiply the one row of a matrix by t, the determinant is multiply by t:$$
\begin{bmatrix}
ta & tb\\c &d 
\end{bmatrix}=t\begin{bmatrix}a & b\\ c & d\end{bmatrix}
$$
   * (b) The determinant behaves like a linear function on the rows of the matrix:$$
\begin{bmatrix}
a+a' &b+b' \\c & d
\end{bmatrix}=\begin{bmatrix}
a & b\\c &d
\end{bmatrix}+\begin{bmatrix}
a' &b' \\
0 & 0
\end{bmatrix}
$$
4.  If two rows of a matrix are equal, its determinant is zero.

![[Pasted image 20241209183935.png]]

![[Pasted image 20241209183511.png]]
## Elimination won't change the determinant(if no row exchange)
![[Pasted image 20241209184047.png]]
![[Pasted image 20241209184108.png]]
![[Pasted image 20241209184315.png]]
	![[Pasted image 20241209184448.png]]![[Pasted image 20241209184612.png]]![[Pasted image 20241209184903.png]]