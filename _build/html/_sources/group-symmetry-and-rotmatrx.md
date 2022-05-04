# Group Symmetry and Rotation Matrices

## The Trace Rule for rotation matrices

If a matrix $R$ is a rotation in 3D, then the angle $\theta$ of the rotation it performs is given by:

$$
tr(R) = 1+2 \cos\theta
$$

The [trace of a matrix](https://textbooks.math.gatech.edu/ila/characteristic-polynomial.html#definition-47) is the sum along its diagonal. For any $n \times n$ matrix: 

$$
tr(a) =\overset{n}{\sum_{\substack i = 1}} = a_{ii}
$$

So, for an example matrix:

$$
\begin{bmatrix}

-1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & -1
\end{bmatrix}
$$

The trace is -1 + 1 + -1 = -1, therefore:

$$
1 + 2\cos \theta = -1
$$

$$
\cos \theta = -1
$$

$$
\theta = 180\\ \textnormal{ so our example matrix represents a rotation of 180\degree}
$$

# From Point Groups to Space Groups

### Rotations with partial translation components

A particular point group can give rise to several space group symmetries if one or more of the pure rotational operators is turned into a screw operation, which is a combination of a rotation with a translational shift a fraction of the distance along the unit cell along which the axis lies.

structure factor
