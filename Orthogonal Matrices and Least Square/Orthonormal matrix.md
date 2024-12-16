#### $\quad$if the columns of the $Q = [q_{1} \dots q_{n}]$ are orthogonal, then $Q^TQ=I$ is the identity.
Matrices with orthonormal columns are **orthonormal matrices**

A **square** orthonormal matrix Q is called an orthogonal matrix. 
- then $Q^TQ=I$ tells us that  $Q^T=Q^{-1}$

For example, if $Q=\begin{bmatrix}0 & 0 & 1\\1 & 0 & 0 \\ 0 & 1 &0\end{bmatrix}$then $Q^T=\begin{bmatrix}0 &1 & 0\\0 & 0 & 1\\1 &0 & 0\end{bmatrix}$.Both $Q$ and $Q^T$ are orthogonal matrices ,and their product is the identity. 

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
  * $B(or\,e)=b-p=b-A(A^TA)^{-1}A^Tb$.
- from orthogonal vectors $A,B$ to **orthonormal** vectors $q_{1},q_{2}$.
  - $q_{1}=\frac{A}{|A|},q_{2}=\frac{B}{|B|}$
  - 