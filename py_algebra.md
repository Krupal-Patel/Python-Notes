# Visualizing Matrix Multiplication
In the videos on *__Linear Transformation and Matrices__*, you learned how a vector can be decomposed into it's basis vectors $\hat{i}$ and $\hat{j}$. 
You also learned that you can tranform a vector by multiplying that vector's $x$ and $y$ values by the *transformed* basis vectors, $\hat{i_T}$ and $\hat{j_T}$, summing their results (see *Equation 1*).

$\hspace{1cm}\textit{transformed } \vec{v} = x\mathbin{\color{green}{\hat{i_T}}} +\, y\, \mathbin{\color{red}{\hat{j_T}}} $

$\hspace{2.3cm}$*Equation 1*


You learned how this method of transforming a vector through use of the *transformed* basis vectors is the same as matrix multiplication (see *Equation 2*).

$\hspace{1cm} \begin{bmatrix} \mathbin{\color{green}a} & \mathbin{\color{red}b}\\ \mathbin{\color{green}c} & \mathbin{\color{red}d} \end{bmatrix} \begin{bmatrix} x\\ y\end{bmatrix} = x \begin{bmatrix}\mathbin{\color{green}a}\\ \mathbin{\color{green}c} \end{bmatrix} + y \begin{bmatrix} \mathbin{\color{red}b}\\ \mathbin{\color{red}d} \end{bmatrix} = \begin{bmatrix} \mathbin{\color{green}a}x + \mathbin{\color{red}b}y\\ \mathbin{\color{green}c}x + \mathbin{\color{red}d}y\end{bmatrix}$ 

$\hspace{4.1cm}$*Equation 2*

```Python
# Define vector v 
v = np.array([-1,2])

# Define 2x2 matrix ij
ij = np.array([[3, 1],[1, 2]])

v_t = np.matmul(v,ij)

# Prints vectors v, ij, and v_t
print("\nMatrix ij:", ij, "\nVector v:", v, "\nTransformed Vector v_t:", v_t, sep="\n")
```
