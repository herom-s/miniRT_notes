
A quadric surface is a [Surface](Surface.md) in **ℝ³** defined by a second-degree [Polynomial](Polynomial.md) [Equation](Equation.md). It generalizes [Conic sections](Conic%20sections.md) to three dimensions, having the following form:

```math
m_{xx}x^2 + m_{yy}y^2 + m_{zz}z^2 + 2m_{xy}xy + 2m_{xz}xz + 2m_{yz}yz + 2m_{x}x + 2m_{y}y + 2m_{z}z + m_{0} = 0
```

Notice that this equation has three distinct types of terms: **[Quadratic](Quadratic.md)** ($x^2, y^2, z^2, xy, xz, yz$), **[Linear](Linear.md)** ($x, y, z$), and a **[Constant](Constant.md)** ($m_0$). Each can be naturally encoded in the following [Matrix form](Matrix%20form.md):

```math
\begin{bmatrix} 
x & y & z 
\end{bmatrix} 
\begin{bmatrix} 
m_{xx} & m_{xy} & m_{xz}\\
m_{xy} & m_{yy} & m_{yz}\\ 
m_{xz} & m_{yz} & m_{zz} 
\end{bmatrix} 
\begin{bmatrix} 
x \\ 
y \\ 
z 
\end{bmatrix} 
+ 2
\begin{bmatrix}
m_{x} & m_{y} & m_{z}
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
+ m_{0} = 0
```

Which we can write compactly as:

```math
x^TAx + 2B^Tx + m_{0} = 0
```
```math
x = 
\begin{bmatrix} 
x \\
y \\
z 
\end{bmatrix}
\quad 
A = 
\begin{bmatrix} 
m_{xx} & m_{xy} & m_{xz} \\
m_{xy} & m_{yy} & m_{yz} \\
m_{xz} & m_{yz} & m_{zz}
\end{bmatrix}
\quad 
B =
\begin{bmatrix} 
m_{x} \\
m_{y} \\
m_{z}
\end{bmatrix}
```

Where $x$ is the [Column vector](Column%20vector.md) of variables, $A$ is a 3×3 [Symmetric matrix](Symmetric%20matrix.md) encoding the quadratic coefficients, and $B$ is a [Column vector](Column%20vector.md) of the linear terms.

Notice that the equation still has three separate parts — the quadratic term, the linear term, and the constant. We can elegantly collapse all of them into a single matrix product by lifting $x$ into [Homogeneous coordinates](Homogeneous%20coordinates.md), introducing an augmented 4×4 [Matrix](Matrix.md) **M**.
```math
\begin{bmatrix} 
x & y & z & 1 
\end{bmatrix} 
\begin{bmatrix} 
m_{xx} & m_{xy} & m_{xz} & m_{x}\\
m_{xy} & m_{yy} & m_{yz} & m_{y}\\
m_{xz} & m_{yz} & m_{zz} & m_{z}\\
m_{x} & m_{y} & m_{z} & m_{0}
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z \\
1
\end{bmatrix}
= 0
```

Which we write as:

$$\hat{x}^TM\hat{x} = 0$$
```math
\hat{x} =
\begin{bmatrix}
x \\
y \\
z \\
1
\end{bmatrix}
\quad
M =
\begin{bmatrix}
m_{xx} & m_{xy} & m_{xz} & m_{x}\\
m_{xy} & m_{yy} & m_{yz} & m_{y}\\
m_{xz} & m_{yz} & m_{zz} & m_{z}\\
m_{x} & m_{y} & m_{z} & m_{0}
\end{bmatrix}
```
