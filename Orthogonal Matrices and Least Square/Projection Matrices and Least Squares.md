# head1
## head2
### head3
#### head 4
##### head 5
###### head 6

~~strikethrough~~

*italic*

**bold**

==hightlighting==

**bold and _italic_ text**

***bold and italic text***

[google](https:google.com)

![renko](https://trendspider.com/learning-center/wp-content/uploads/2023/06/Renko-Chart@300x-min.jpg)

>this is a ***quote***

\- me

- 1
- 2
- 3

1. 23
2. 34

- [?] this 
- [x] this
- [-] this

    rm -rf /~
	
```c
#include <iostream>
using namespace std;
int main(){
cout<<"Hello World";
return 0;
}
```

Project matrix:
- $P=A(A^TA)^{-1}A^T$
$$
if\ b\ in\ column\ space \ Pb=b 
$$
$$if \perp Column\ space\ Pb=0$$

if  b in the column space ,then the $b=Ax$.We can get $p = Pb=A(A^TA)^{-1}A^TAx$.

After cancelation we have $p=Ax$
![[Pasted image 20241209102856.png]]

if P is a projection matrix then $(I-P)$ is also projection matrix . it project $e$ on to the **$\perp$ space 
(N($A^T$ )Left null space).
$$
p=Pb
$$
$$
e=(I-P)b
$$
![[Pasted image 20241209110754.png]]

Since error is $\perp$ a,
we have $A^{T}e = 0$,$e=b-p=b-A\hat{x}$
then$A^T(b-A\hat{x})=0,A^TA\hat{x}=A^Tb$


## if you can't solve a $Ax=b$ (often $m>n$)
1. find out the general form of the equation.
2. write it in terms of matrix, the matrix $A$ and vector $b$.
3. set up [[Project equation]] : $A^TA\hat{x}=A^Tb$;
4. solve the $\hat{x}$;
