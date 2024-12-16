>***Many calculations become simpler when performed using orthonormal vectors or orthogonal matrices. In this session, we learn a procedure for converting any basis to an orthonormal one.***

# [[Orthonormal vectors]]
$$
q^T_{i}q_{j}=\begin{cases}
 \ 0\quad if\quad i\neq j \\
 \ 1\quad if\quad i=j
\end{cases}
$$

# [[Orthonormal matrix]]

>if the columns of the $Q = [q_{1} \dots q_{n}]$ are orthogonal, then $Q^TQ=I$ is the identity.

## Orthogonal matrices are good

Suppose $Q$ has orthogonal columns.the [Projection Matrices](obsidian://open?vault=linear%20algebra&file=Projection%20Matrices%20and%20Least%20Squares) of $Q$ is:
$$
P=Q(Q^TQ)Q^T
$$
Since $Q^TQ=I$,$P=QQ^T$.
- If $Q$ is square then $Q^T=Q^{-1}$, $P=I$.
- $A^TA\hat{x}=A^Tb$ becomes $\hat{x}=A^Tb$.

## Gram-Schmidt

With elimination, our goal was “make the matrix triangular”. Now our goal is “**make the matrix orthonormal**”.
![[Pasted image 20241209152418.png]]
* From independent vectors $a,b$ to orthogonal vectors $A,B$.
  * Set $a=A$.
  * Find the vector that is perpendicular to the $A$.
  * It's the error(e)!
  * $B(or\,e)=b-p=b-A(A^TA)^{-1}A^Tb=b-\frac{A^Tb}{A^TA}A$.
  * if there are more than 3 vectors for example c.
  * $C=c-\frac{A^Tc}{A^TA}A-\frac{B^Tc}{B^TB}B$.
  * $\dots$
  * $X=x-\frac{A^Tx}{A^TA}A-\frac{B^Tx}{B^TB}B\dots-\frac{W^Tx}{W^TW}W$
- from orthogonal vectors $A,B$ to **orthonormal** vectors $q_{1},q_{2}$.
  - $q_{1}=\frac{A}{|A|},q_{2}=\frac{B}{|B|}$
  - $Q=\begin{bmatrix}q_{1} &q_{2}\dots qn\end{bmatrix}$

When we studied elimination, we wrote the process in terms of matrices and found A = LU. A similar equation **A = QR** relates our starting matrix A to the result Q of the Gram-Schmidt process. Where L was lower triangular, R is upper triangular.

Suppose $A=\begin{bmatrix}q_{1} & q_{2}\end{bmatrix}$ ,Then:
$$
A\qquad Q\qquad R
$$
$$\qquad
\begin{bmatrix}
a_{1} & a_{2}
\end{bmatrix}=\begin{bmatrix}
q_{1} & q_{2}
\end{bmatrix}\quad\begin{bmatrix}
q_{1}^Ta_{1} &q_{2}^Ta_{1} \\
q_{1}^Ta_{2} &q_{2}^Ta_{2}
\end{bmatrix}
$$
All the later $q_{i}$ were chosen to be perpendicular to the earlier a,

for any $q_{i}^Ta_{j}=0(i<j)$ 

since the $A=QR$,and Q has orthonormal columns,$Q^TQ=I$.

multiple both side by $Q^T$ get the $Q^TA=Q^TQR$

so $Q^TA=R$

Therefore $R=Q^TA$.