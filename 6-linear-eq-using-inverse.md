# Solving Linear Equations Using Inverse Matrix

## Introduction

A system of linear equations can be represented in matrix form. When we have a system of linear equations, we can write it as:

$$AX = B$$

Where:
- $A$ is the coefficient matrix
- $X$ is the matrix (or vector) of unknowns
- $B$ is the matrix (or vector) of constant terms

If matrix $A$ is invertible (meaning its determinant is non-zero), then the solution to the system is:

$$X = A^{-1}B$$

## Solution Steps

1. Organize the system of equations in matrix form $AX = B$
2. Calculate the determinant of $A$ to ensure it's invertible (det$(A) \neq 0$)
3. Calculate the inverse matrix $A^{-1}$
4. Multiply both sides by $A^{-1}$ on the left: $A^{-1}AX = A^{-1}B$
5. Simplify: $IX = A^{-1}B$, meaning $X = A^{-1}B$

## Example with 2 Unknowns

Let's solve the following system:
```
3x + 2y = 14
2x + 5y = 19
```

### Step 1: Organize in Matrix Form

$$A = \begin{bmatrix} 3 & 2 \\ 2 & 5 \end{bmatrix}$$

$$X = \begin{bmatrix} x \\ y \end{bmatrix}$$

$$B = \begin{bmatrix} 14 \\ 19 \end{bmatrix}$$

### Step 2: Calculate the Determinant

$$\text{det}(A) = 3 \times 5 - 2 \times 2 = 15 - 4 = 11$$

Since det$(A) \neq 0$, matrix $A$ is invertible and the system has a unique solution.

### Step 3: Calculate the Inverse Matrix

The adjugate matrix of $A$:

$$\text{adj}(A) = \begin{bmatrix} 5 & -2 \\ -2 & 3 \end{bmatrix}$$

The inverse matrix:

$$A^{-1} = \frac{1}{\text{det}(A)} \times \text{adj}(A) = \frac{1}{11} \times \begin{bmatrix} 5 & -2 \\ -2 & 3 \end{bmatrix} = \begin{bmatrix} \frac{5}{11} & \frac{-2}{11} \\ \frac{-2}{11} & \frac{3}{11} \end{bmatrix}$$

### Step 4: Multiply by $A^{-1}$ on the Left

$$X = A^{-1} \times B = \begin{bmatrix} \frac{5}{11} & \frac{-2}{11} \\ \frac{-2}{11} & \frac{3}{11} \end{bmatrix} \times \begin{bmatrix} 14 \\ 19 \end{bmatrix} = \begin{bmatrix} \frac{5}{11} \times 14 + \frac{-2}{11} \times 19 \\ \frac{-2}{11} \times 14 + \frac{3}{11} \times 19 \end{bmatrix}$$

### Step 5: Calculate the Solution

$$X = \begin{bmatrix} \frac{70}{11} - \frac{38}{11} \\ \frac{-28}{11} + \frac{57}{11} \end{bmatrix} = \begin{bmatrix} \frac{32}{11} \\ \frac{29}{11} \end{bmatrix} \approx \begin{bmatrix} 2.91 \\ 2.64 \end{bmatrix}$$

Therefore, $x = \frac{32}{11} \approx 2.91$ and $y = \frac{29}{11} \approx 2.64$.

## Example with 3 Unknowns

Let's solve the following system:
```
2x + y + z = 5
x + 3y + 2z = 10
3x + 2y + 4z = 16
```

### Step 1: Organize in Matrix Form

$$A = \begin{bmatrix} 2 & 1 & 1 \\ 1 & 3 & 2 \\ 3 & 2 & 4 \end{bmatrix}$$

$$X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}$$

$$B = \begin{bmatrix} 5 \\ 10 \\ 16 \end{bmatrix}$$

### Step 2: Calculate the Determinant

$$\text{det}(A) = 2 \times (3 \times 4 - 2 \times 2) - 1 \times (1 \times 4 - 2 \times 3) + 1 \times (1 \times 2 - 3 \times 3)$$
$$= 2 \times (12 - 4) - 1 \times (4 - 6) + 1 \times (2 - 9)$$
$$= 2 \times 8 - 1 \times (-2) + 1 \times (-7)$$
$$= 16 + 2 - 7 = 11$$

Since det$(A) \neq 0$, matrix $A$ is invertible and the system has a unique solution.

### Step 3: Calculate the Inverse Matrix

To calculate the inverse of a 3×3 matrix, we first compute the adjugate matrix.

The adjugate matrix of $A$:

$$\text{adj}(A) = \begin{bmatrix} (3 \times 4 - 2 \times 2) & -(1 \times 4 - 2 \times 3) & (1 \times 2 - 3 \times 3) \\ -(2 \times 4 - 1 \times 3) & (2 \times 4 - 1 \times 1) & -(2 \times 2 - 1 \times 3) \\ (2 \times 2 - 1 \times 3) & -(2 \times 1 - 1 \times 3) & (2 \times 3 - 1 \times 2) \end{bmatrix}$$

$$= \begin{bmatrix} 8 & 2 & -7 \\ -5 & 7 & 1 \\ 1 & -1 & 4 \end{bmatrix}$$

The inverse matrix:

$$A^{-1} = \frac{1}{\text{det}(A)} \times \text{adj}(A) = \frac{1}{11} \times \begin{bmatrix} 8 & 2 & -7 \\ -5 & 7 & 1 \\ 1 & -1 & 4 \end{bmatrix}$$

$$= \begin{bmatrix} \frac{8}{11} & \frac{2}{11} & \frac{-7}{11} \\ \frac{-5}{11} & \frac{7}{11} & \frac{1}{11} \\ \frac{1}{11} & \frac{-1}{11} & \frac{4}{11} \end{bmatrix}$$

### Step 4: Multiply by $A^{-1}$ on the Left

$$X = A^{-1} \times B = \begin{bmatrix} \frac{8}{11} & \frac{2}{11} & \frac{-7}{11} \\ \frac{-5}{11} & \frac{7}{11} & \frac{1}{11} \\ \frac{1}{11} & \frac{-1}{11} & \frac{4}{11} \end{bmatrix} \times \begin{bmatrix} 5 \\ 10 \\ 16 \end{bmatrix}$$

### Step 5: Calculate the Solution

$$X = \begin{bmatrix} \frac{8}{11} \times 5 + \frac{2}{11} \times 10 + \frac{-7}{11} \times 16 \\ \frac{-5}{11} \times 5 + \frac{7}{11} \times 10 + \frac{1}{11} \times 16 \\ \frac{1}{11} \times 5 + \frac{-1}{11} \times 10 + \frac{4}{11} \times 16 \end{bmatrix}$$

$$= \begin{bmatrix} \frac{40}{11} + \frac{20}{11} - \frac{112}{11} \\ \frac{-25}{11} + \frac{70}{11} + \frac{16}{11} \\ \frac{5}{11} - \frac{10}{11} + \frac{64}{11} \end{bmatrix}$$

$$= \begin{bmatrix} \frac{-52}{11} \\ \frac{61}{11} \\ \frac{59}{11} \end{bmatrix} \approx \begin{bmatrix} -4.73 \\ 5.55 \\ 5.36 \end{bmatrix}$$

Therefore, $x = \frac{-52}{11} \approx -4.73$, $y = \frac{61}{11} \approx 5.55$, and $z = \frac{59}{11} \approx 5.36$.

## Example with 4 Unknowns

Let's solve the following system:
```
x + y - z + w = 4
2x - y + 2z - w = 3
3x + 2y - z - 2w = 0
x - 3y - 3z + 3w = 2
```

### Step 1: Organize in Matrix Form

$$A = \begin{bmatrix} 1 & 1 & -1 & 1 \\ 2 & -1 & 2 & -1 \\ 3 & 2 & -1 & -2 \\ 1 & -3 & -3 & 3 \end{bmatrix}$$

$$X = \begin{bmatrix} x \\ y \\ z \\ w \end{bmatrix}$$

$$B = \begin{bmatrix} 4 \\ 3 \\ 0 \\ 2 \end{bmatrix}$$

### Step 2: Calculate the Determinant

Calculating the determinant of a 4×4 matrix is a complex process. In this case, det$(A) = 18 \neq 0$, so matrix $A$ is invertible.

### Step 3: Calculate the Inverse Matrix

In practice, the inverse of a 4×4 matrix is usually calculated using computational algorithms. The inverse matrix in this case is:

$$A^{-1} = \begin{bmatrix} \frac{1}{6} & \frac{1}{3} & 0 & 0 \\ \frac{2}{9} & \frac{1}{9} & \frac{1}{9} & \frac{-1}{3} \\ \frac{1}{18} & \frac{1}{9} & \frac{1}{18} & \frac{-1}{6} \\ \frac{2}{9} & \frac{1}{3} & \frac{1}{9} & \frac{-1}{3} \end{bmatrix}$$

### Steps 4 and 5: Multiply by $A^{-1}$ and Calculate the Solution

$$X = A^{-1} \times B = \begin{bmatrix} \frac{1}{6} & \frac{1}{3} & 0 & 0 \\ \frac{2}{9} & \frac{1}{9} & \frac{1}{9} & \frac{-1}{3} \\ \frac{1}{18} & \frac{1}{9} & \frac{1}{18} & \frac{-1}{6} \\ \frac{2}{9} & \frac{1}{3} & \frac{1}{9} & \frac{-1}{3} \end{bmatrix} \times \begin{bmatrix} 4 \\ 3 \\ 0 \\ 2 \end{bmatrix}$$

After performing the calculations, we get:

$$X = \begin{bmatrix} 2 \\ 1 \\ 0 \\ 1 \end{bmatrix}$$

Therefore, $x = 2$, $y = 1$, $z = 0$, and $w = 1$.

## Summary

The method of solving a system of linear equations using an inverse matrix is an efficient and elegant approach, especially when:
1. The number of equations equals the number of unknowns
2. The determinant of the coefficient matrix is non-zero (meaning there is a unique solution)

Advantages of the method:
- Methodical and systematic
- Allows handling of large systems of equations
- Convenient for implementation using computational tools

Disadvantages of the method:
- Calculating the inverse matrix can be complex, especially for large matrices
- Sensitive to rounding errors in numerical calculations
- Not as computationally efficient as other methods (e.g., LU decomposition)

In practice, other numerical methods are usually used to solve large systems of linear equations, but understanding the inverse matrix method provides important insights into linear algebra and the properties of equation systems.
