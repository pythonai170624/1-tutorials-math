# Matrix Properties with Examples

## 1. c(A + B) = cA + cB
This property states that multiplication of a scalar by a sum of matrices equals the sum of the scalar multiplied by each matrix individually.

### Example:
Let's define matrices A and B:

Matrix A = $\begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix}$

Matrix B = $\begin{pmatrix} 5 & 6 \\\\ 7 & 8 \end{pmatrix}$

And let c = 3

**Left side:** c(A + B)
1. First, find A + B:
   $A + B = \begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix} + \begin{pmatrix} 5 & 6 \\\\ 7 & 8 \end{pmatrix} = \begin{pmatrix} 6 & 8 \\\\ 10 & 12 \end{pmatrix}$
   
2. Then multiply by c:
   $c(A + B) = 3 \begin{pmatrix} 6 & 8 \\\\ 10 & 12 \end{pmatrix} = \begin{pmatrix} 18 & 24 \\\\ 30 & 36 \end{pmatrix}$

**Right side:** cA + cB
1. First, multiply each matrix by c:
   $cA = 3 \begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 3 & 6 \\\\ 9 & 12 \end{pmatrix}$
   
   $cB = 3 \begin{pmatrix} 5 & 6 \\\\ 7 & 8 \end{pmatrix} = \begin{pmatrix} 15 & 18 \\\\ 21 & 24 \end{pmatrix}$
   
2. Then add the results:
   $cA + cB = \begin{pmatrix} 3 & 6 \\\\ 9 & 12 \end{pmatrix} + \begin{pmatrix} 15 & 18 \\\\ 21 & 24 \end{pmatrix} = \begin{pmatrix} 18 & 24 \\\\ 30 & 36 \end{pmatrix}$

Both sides equal $\begin{pmatrix} 18 & 24 \\\\ 30 & 36 \end{pmatrix}$, confirming that c(A + B) = cA + cB.

## 2. (c + d)A = cA + dA
This property states that the sum of scalars multiplied by a matrix equals the sum of each scalar multiplied by the matrix individually.

### Example:
Let's define matrix A:

Matrix A = $\begin{pmatrix} 2 & 3 \\\\ 4 & 5 \end{pmatrix}$

And let c = 2 and d = 3

**Left side:** (c + d)A
1. First, add the scalars:
   c + d = 2 + 3 = 5
   
2. Then multiply the matrix by this sum:
   $(c + d)A = 5 \begin{pmatrix} 2 & 3 \\\\ 4 & 5 \end{pmatrix} = \begin{pmatrix} 10 & 15 \\\\ 20 & 25 \end{pmatrix}$

**Right side:** cA + dA
1. Multiply the matrix by each scalar:
   $cA = 2 \begin{pmatrix} 2 & 3 \\\\ 4 & 5 \end{pmatrix} = \begin{pmatrix} 4 & 6 \\\\ 8 & 10 \end{pmatrix}$
   
   $dA = 3 \begin{pmatrix} 2 & 3 \\\\ 4 & 5 \end{pmatrix} = \begin{pmatrix} 6 & 9 \\\\ 12 & 15 \end{pmatrix}$
   
2. Then add the results:
   $cA + dA = \begin{pmatrix} 4 & 6 \\\\ 8 & 10 \end{pmatrix} + \begin{pmatrix} 6 & 9 \\\\ 12 & 15 \end{pmatrix} = \begin{pmatrix} 10 & 15 \\\\ 20 & 25 \end{pmatrix}$

Both sides equal $\begin{pmatrix} 10 & 15 \\\\ 20 & 25 \end{pmatrix}$, confirming that (c + d)A = cA + dA.

## 3. c(dA) = (cd)A
This property states that multiplying a matrix by scalar d and then by scalar c is equivalent to multiplying the matrix by the product of the two scalars.

### Example:
Let's define matrix A:

Matrix A = $\begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix}$

And let c = 2 and d = 3

**Left side:** c(dA)
1. First, multiply A by d:
   $dA = 3 \begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 3 & 6 \\\\ 9 & 12 \end{pmatrix}$
   
2. Then multiply the result by c:
   $c(dA) = 2 \begin{pmatrix} 3 & 6 \\\\ 9 & 12 \end{pmatrix} = \begin{pmatrix} 6 & 12 \\\\ 18 & 24 \end{pmatrix}$

**Right side:** (cd)A
1. First, multiply the scalars:
   cd = 2 × 3 = 6
   
2. Then multiply the matrix by this product:
   $(cd)A = 6 \begin{pmatrix} 1 & 2 \\\\ 3 & 4 \end{pmatrix} = \begin{pmatrix} 6 & 12 \\\\ 18 & 24 \end{pmatrix}$

Both sides equal $\begin{pmatrix} 6 & 12 \\\\ 18 & 24 \end{pmatrix}$, confirming that c(dA) = (cd)A.

## 4. 1A = A
This property states that multiplying a matrix by the scalar 1 returns the original matrix.

### Example:
Let's define matrix A:

Matrix A = $\begin{pmatrix} 5 & 7 \\\\ 2 & 9 \end{pmatrix}$

**Calculation:** 1A
$1A = 1 \begin{pmatrix} 5 & 7 \\\\ 2 & 9 \end{pmatrix} = \begin{pmatrix} 5 & 7 \\\\ 2 & 9 \end{pmatrix} = A$

This confirms that 1A = A.

## 5. 0A = 0 (Zero Matrix)
This property states that multiplying any matrix by the scalar 0 results in a zero matrix of the same dimensions.

### Example:
Let's define matrix A:

Matrix A = $\begin{pmatrix} 4 & 8 \\\\ 3 & 5 \end{pmatrix}$

**Calculation:** 0A
$0A = 0 \begin{pmatrix} 4 & 8 \\\\ 3 & 5 \end{pmatrix} = \begin{pmatrix} 0 & 0 \\\\ 0 & 0 \end{pmatrix}$

This confirms that 0A equals a zero matrix of the same dimensions as A.

## 6. (-1)A = -A
This property states that multiplying a matrix by -1 is equivalent to negating each element of the matrix.

### Example:
Let's define matrix A:

Matrix A = $\begin{pmatrix} 2 & -3 \\\\ 5 & 1 \end{pmatrix}$

**Left side:** (-1)A
$(-1)A = (-1) \begin{pmatrix} 2 & -3 \\\\ 5 & 1 \end{pmatrix} = \begin{pmatrix} -2 & 3 \\\\ -5 & -1 \end{pmatrix}$

**Right side:** -A
$-A = -\begin{pmatrix} 2 & -3 \\\\ 5 & 1 \end{pmatrix} = \begin{pmatrix} -2 & 3 \\\\ -5 & -1 \end{pmatrix}$

Both sides equal $\begin{pmatrix} -2 & 3 \\\\ -5 & -1 \end{pmatrix}$, confirming that (-1)A = -A.
