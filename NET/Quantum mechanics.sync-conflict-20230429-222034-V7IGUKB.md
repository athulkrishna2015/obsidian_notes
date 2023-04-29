# Particle wave
## non relativistic
- $\lambda = \frac{h}{p}$
- $\lambda = \frac{h}{\sqrt{2mK.E}}$,
	- $KE=\frac{p^2}{2m}$
	- $KE=qV$
		- $\lambda= \frac{12.27 A^o}{\sqrt{V}}$
	- $K.E=\frac{f}{2}K_BT$, Thermal Energy,f= degree of freedom
## relativistic [[Classical Mechanics#Special theory of relativty]]
$\lambda =\frac{h}{\sqrt{2mK.E\left(1+\frac{K.E}{2m_0c^2} \right)}}$

compton effect  
$\Delta \lambda = \frac{h}{m_0 c }(1-\cos \phi)$
- $p=-i\hbar \nabla$
- $KE = \frac{-\hbar^2}{2m}\nabla^2$
- $E=i\hbar \frac{\partial}{\partial t}$
  
  - Dispersion relation $v_g =v_p -\lambda \frac{dv_p}{d\lambda}$,group velocity
	 -  $\frac{dv_p}{d\lambda} = 0$ in non dispersive medium  
	 -  $\frac{dv_p}{d\lambda} > 0$ Normal dispesion
	   -  $\frac{dv_p}{d\lambda} < 0$ Anomalous dispersion
# wave function
$\psi(r,t) = Ae^{i(k\dot r - \omega t)}$
$\psi $ and its derivatives must be continuous, Single valued, square integrable,   

### operators as functions
- $\hat{p}=-i\hbar \nabla$
- $\hat{K.E}=-\frac{\hbar^2}{2m}\nabla^2$
- $\hat{E}=i\hbar \frac{d}{dt}$
- $\hat{H}=-\frac{\hbar^2}{2m}\nabla^2+U$
- $\hat{L}=\hat{r}\times \hat{p}$
- Expectation value $<A>=\frac{\int \psi^* \hat{A} \psi}{\psi^*\psi}$

## Dirac notation
$<\psi|=(|\psi>^\intercal)^*$
### Inner product
- $<\psi_1|\psi_2> = <\psi_2|\psi_1>^*$
- $\int_{-\infty}^\infty \psi_1^*\psi_2 = (\int_{-\infty}^\infty \psi_1^*\psi_1)^*$
- $<\phi_1|\phi_2> = \delta_{i,j}$
- $|\psi>=\Sigma_1^n c_n|\phi_n>$
	- $|\psi>=\Sigma_1^n c_n^*<\phi_n|$
Schwartz inequality
$(<\psi|\phi>)^2\leq |<\psi|\psi>||<\phi|\phi>|$

### Probability
$P_i= \frac{|<\phi_i|\psi>|^2}{<\psi|\psi>}$

### Operator
- $\hat{A}|\psi>=a|\psi>$, a is eigen value, $\psi$ = eigen state
- Expectation value $<A>=\frac{<\psi|A|\psi>}{<\psi|\psi>}$(average value)
	- $<A>=\Sigma p_i a_i$, Only applicable when basis vectors are eigen state of the operator 
		- $<E>=\Sigma p_i \epsilon_i$

## Schrodinger equation 
- $i\hbar \frac{\partial \psi}{\partial t}= \frac{-\hbar^2}{2m}\nabla^2\psi + U(\psi)$
- $\nabla^2 \phi + \frac{2m}{\hbar^2}(E-U)\phi = 0$


- continuity equation $\nabla \cdot S + \frac{\partial P}{\partial t} = 0$
	- Probability current density $S= \frac{\hbar}{2im} [\psi^* \nabla \psi - \psi^ \nabla \psi^*$]
	- $S=Re(\psi^*\hat{V}\psi$) where $\hat{V}=\hat{p}/m$ velocity 
	- probability density $P=\psi^*\psi$

## Particle in a box
1D
- $\psi_n(x)=\sqrt{\frac{2}{a}}\sin \frac{n\pi x}{a}$
- $E_n=\frac{n^2\hbar^2\pi^2}{2ma^2}$
3D
- $\psi_n(x)=\sqrt{\frac{8}{abc}}\sin \frac{n_x\pi x}{a}\sin \frac{n_y\pi x}{b}\sin \frac{n_z\pi x}{c}$
- $E_{n_xn_yn_z}=\frac{\hbar^2\pi^2}{2m}\left(\frac{n^2_x}{a}+\frac{n^2_y}{b}+\frac{n^2_z}{c}\right)$
## Bohr model of atom
- $r_n=\frac{n^2h^2\epsilon_0}{\pi Z me^2}= 0.529 \frac{n^2}{Z} A^o$, n= principle quantum number
- $E_n=\frac{Z^2me^4} {8n^2h^2\epsilon_0^2}=-13.6\frac{Z^2}{n}eV$

Hydrogen spectra
$\frac{1}{\lambda}=R\left[\frac{1}{n_1}-\frac{1}{n_2} \right]$, R= Rydburg const.
- L - UV
- B - Visible
- P,B,P - IR

# Nuclear
- $R=R_0A^{\frac{1}{3}}$,$R_0=1.1 - 1.2 fm$
- 
## Radio activity
- $N=N_oe^{-\lambda t}$
	- $\frac{dN}{dt}=-\lambda N_0$
- $t_{\frac{1}{2}}=\frac{ln(2)}{\lambda}=\frac{.629}{\lambda}$
- mean life time $\tau=\frac{1}{\lambda}$




