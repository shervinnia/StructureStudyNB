# Optical Transforms and Structure Factor Convolutions

# The “Big Picture” of Diffraction

$$

\begin{CD}
\normalsize{\large\blacksquare}\atop\small\textnormal{Crystal}\space [I(h,k,l)]\\
@VF=T[\rho]V\textnormal Fourier AnalysisV \\
F_{obs}(h,k,l) @>\rho=T[F]>\textnormal{Fourier Synthesis}> \normalsize{\large\blacksquare}\atop\small\textnormal{Electron Density Map}\\
@VVV @VF=T[\rho]V\textnormal{Fourier Analysis}V\\
R = \frac{\Sigma{|F_{obs}-F_{calc}}|}{\Sigma{F_{obs}}} @<<< F_{calc}(h,k,l)
\end{CD}
$$

$R$    Calculates the accuracy of the constructed model compared to experimental observation. Though, the experimental observation is also expected to not be perfect.

$$
\overrightharpoon{F}(h,k,l) = \Sigma\textcolor{#2980B9}{\overrightharpoon{f_j}} = \Sigma\textcolor{#2980B9}{f_j}\textcolor{#27AE60}{e^{i\phi_j}}=\Sigma \textcolor{#2980B9}{f_j}\textcolor{#27AE60}{[cos\phi_j+i\space sin\phi_j]}
$$

### Structure Factors

Structure Factors [  $\overrightharpoon{F}(h,k,l)$  ]   represent a sum of all of the scattered wavelets from each atom in the unit cell.

### Scattering Factors

$f_j$  is the atomic scattering factor of atom $j$. It’s value is dependent on the number of electrons of the atom and the extent of the atom’s motion.

### Euler’s Formula

$e^{i\phi}=cos\phi + i\space sin\phi$

# Convolution

Convolution is the process of placing one function (the ‘motif’) atop every point of another function.
