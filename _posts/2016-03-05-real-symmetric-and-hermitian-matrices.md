---
layout: post
title: Real symmetric and Hermitian matrices 
---

Symmetric and Hermitian matrices are properties of two classes of matrices 
found in applications that naturally give rise to matrices of symmetric or 
Hermitian structure. Here, we take a brief look at what these properties 
are and how to use them.

In this post, we explore symmetric matrices from the basic case moving 
into the real and complex cases. As always, the lack of rigorosity and 
proofs are apparent.

---




## Symmetric

Symmetric matrices are square matrices that are equal to their transpose

$$ A = A^{T} $$

Symmetric in this sense means that elements are reflected about the matrix 
diagonal. Consequently, diagonal matrices are always symmetric:

$$ 
A = 
\begin{bmatrix}
    \lambda_1 & 0 \\
    0 & \lambda_2
\end{bmatrix}
=
A^T
=
\begin{bmatrix}
    \lambda_1 & 0 \\
    0 & \lambda_2
\end{bmatrix}
$$

Not all transposed matrices are symmetric, since for example:

$$ 
A = 
\begin{bmatrix}
    a_{11} & a_{12} \\
    a_{21} & a_{22} \\
    a_{31} & a_{32} \\
\end{bmatrix}
=
A^T
=
\begin{bmatrix}
    a_{11} & a_{21} & a_{31} \\ 
    a_{12} & a_{22} & a_{32} \\
\end{bmatrix}
$$

is a valid transposition operation.

### Real symmetric 

The definition of real symmetric matrices is

$$
\langle Ax, y \rangle = \langle x, Ay \rangle \;\; \forall x,y \in \mathbb{R}^n
$$

For example, with

$$ 
x = 
\begin{bmatrix}
     x_{1} \\
     x_{2} \\
\end{bmatrix}
A = 
\begin{bmatrix}
    a_{1} & a_{2} \\
    a_{2} & a_{3} \\
\end{bmatrix}
y =
\begin{bmatrix}
     y_{1} \\
     y_{2} \\
\end{bmatrix}
$$

we have

$$ 
Ax = 
\begin{bmatrix}
     a_1x_1+a_2x_2 \\
     a_2x_1+a_3x_2 \\
\end{bmatrix}
Ay = 
\begin{bmatrix}
     a_1y_1+a_2y_2 \\
     a_2y_1+a_3y_2 \\
\end{bmatrix}
$$

The inner products are 

$$
    \langle Ax, y \rangle = y_1(a_1x_1+a_2x_2) + y_2(a_2x_1+a_3x_2) \\
    \langle x, Ay \rangle = x_1(a_1y_1+a_2y_2) + x_2(a_2y_1+a_3y_2) 
$$

which is equal. In the non-symmetric case, $$ a_{21} = a_4 \neq a_2 $$ we get

$$
    \langle Ax, y \rangle = y_1(a_1x_1+a_2x_2) + y_2(a_4x_1+a_3x_2) \\
    \langle x, Ay \rangle = x_1(a_1y_1+a_2y_2) + x_2(a_4y_1+a_3y_2) 
$$

not equal.

> As a note, according to the spectral theorem, any real symmetric matrix can be diagonalized by an orthogonal matrix $$ D = \Lambda^T A \Lambda $$ for $$A$$ real symmetric, $$D$$ diagonal and $$\Lambda$$ orthogonal.

## Hermitian

In this discussion we will glance over complex symmetric matrices and continue directly 
with the Hermitian matrix.

The Hermitian property extends symmetry to symmetric matrices with complex entries

$$ 
    A = \overline{A^T}= A^{\dagger}
$$

or 

$$ 
    a_{ij} = \overline{a_{ji}}
$$

An immediate observation is that the diagonal elements of every Hermitian matrix is 
necessarily real since they must be equal to their copmlex conjugate. 

<div class="message">
This post will be updated continously
</div>



