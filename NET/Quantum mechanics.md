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
$\psi(r,t) = Ae^{i(k\cdot r - \omega t)}$
$\psi$ and its derivatives must be continuous, Single valued, square integrable,
$\psi(x,t)=Ae^{\frac{-i}{\hbar}(Et-px)}$
$\psi(x,t)=\phi(x)f(t)$ ,where $f{t}=e^{\frac{-i}{\hbar}Et}$


### operators as functions
- $\hat{p}=-i\hbar \nabla$
- $\hat{K.E}=-\frac{\hbar^2}{2m}\nabla^2$
- $\hat{E}=i\hbar \frac{d}{dt}$
- $\hat{H}=-\frac{\hbar^2}{2m}\nabla^2+U$
- $\hat{L}=\hat{r}\times \hat{p}$
- Expectation value $<A>=\frac{\int \psi^* \hat{A} \psi}{\psi^*\psi}$
	- $<A>=\frac{<\psi|\hat{A}|\psi>}{<\psi|\psi>}$

## Dirac notation
$<\psi|=(|\psi>^\intercal)^*$
### Inner product
- $<\psi_1|\psi_2> = <\psi_2|\psi_1>^*$
- $\int_{-\infty}^\infty \psi_1^*\psi_2 = (\int_{-\infty}^\infty \psi_2^*\psi_1)^*$
- $<\phi_1|\phi_2> = \delta_{i,j}$
- $|\psi>=\Sigma_1^n c_n|\phi_n>$
	- $|\psi>=\Sigma_1^n c_n^*<\phi_n|$

Schwartz inequality
$(<\psi|\phi>)^2\leq |<\psi|\psi>||<\phi|\phi>|$


### Probability
$P_i= \frac{|<\phi_i|\psi>|^2}{<\psi|\psi>}$


commuatative
 $AB=BA$ [A,B] = AB-BA
anticammutative
 $AB=-BA$

- $[x,p_x]=i\hbar$
	- $[x,P]=i\hbar$
- if two operator are Hermitian and their product is also Hermitian then they are commutative
- $[A,B]^\dagger = [B^\dagger,A^\dagger]$
	- if $A^\dagger = A \text{ and } B^\dagger = A$
	- $[A,B]^\dagger = -[A,B]$
- [A, B+C+D] = [A,B]+[A,C]+[A,D]
- Distributive [A,BC] = [A,B]C+B[A,C]
- Jacabi identity [A,[B,C]]+[B,[C,A]]+[C,[A,B]]=0
- $[A,B^n]=nB^{n-1}[A,B]$, or  $[A^n,B]=nA^{n-1}[A,B]$
- Tr[A,B]=0 , Tr(AB)=Tr[BA]
- [f(A),(g(A))]=0, also [f(A),f(B)=0], if [A,B]=0


### Operator
- $\hat{A}|\psi>=a|\psi>$, a is eigen value, $\psi$ = eigen state
	- $H|\psi>=E|\psi>$
- Expectation value $<A>=\frac{<\psi|A|\psi>}{<\psi|\psi>}$(average value)
	- $<A>=\Sigma p_i a_i$, Only applicable when basis vectors are eigen state of the operator 
		- $<E>=\Sigma p_i \epsilon_i$
#### Hermitian operator
- $<f|A|g> = <fB|g>$ B is Hermitian adjoint of A  ($B=A^\dagger$)
 - $<f|Ag> = $<A^\dagger f|g>$
 - $\int_{-\infty}^{\infty} f^* \hat{A} g dx =\int_{-\infty}^{\infty} (A^\dagger f)^* g dx$

- if $A^\dagger = A$ then A is Hermitian operator
- operators associated with physical quantities are Hermitian
 - $i^\dagger = -i$
- The eigen values of an hermitian operators are real and the corresponding eigen vectors are orthogonal
	-  The eigen values of an Anti-hermitian operators are Zero or imaginary and the corresponding eigen vectors are orthogonal

#### Projection operator
- $p^2 = p$
- $p^\dagger = p$
- eigen value is zero or one
- the product of two commuting projection operator is also a projection operator
	 - $[P_1,P_2]= 0$, $P_1P_2 = P_2P_1$
- sum of two projection operator is also a projection operator if they are anti-commutative
	 - $P_1P_2 = -P_2P_1$
#### Angular momentum operator
- $\hat{L}=\vec{r} \times \vec{p}$
	- $L_x=yP_z-zP_y$
	- $L_y=zP_x-xP_z$
	- $L_z=xP_y-yP_z$
![[Screenshot_20230426_182722.png]]

#### Inverse operator 
- $B=A^{-1}$
	- $AB=I$
- $A|\psi>=\lambda |\psi>$
	- $A^{-1}|\psi>=\frac{1}{\lambda} |\psi>$
##### unitary operator
- $A^\dagger = A^{-1}$ or $AA^\dagger=I$
- product of unitary operators is also a unitary operator
- Eigen value of unitary operator is complex number of modulus =1
- Eigen vectors of a unitary operator that has non degenerate eigen values are orthogonal

## Uncertainty relation 

$\Delta A \Delta B =\frac{1}{2}|<[A,B]>|$
- $\Delta A \geq \sqrt{<A^2>-<A>^2}$ 

### Hermitian function
${f(A)}^\dagger = f(A)$
- iff $f$ is real and $A$ is hermitian function

## Schrodinger equation 
- $i\hbar \frac{\partial \psi}{\partial t}= \frac{-\hbar^2}{2m}\nabla^2\psi + U(\psi)$
- $\nabla^2 \phi + \frac{2m}{\hbar^2}(E-U)\phi = 0$

### Solution
$\frac{d^2 \phi}{d x^2} + k^2 x = 0$
contant potential
- (E>V), Unbounded, Oscillatory and imaginary
	-  $\phi = Ae^{ikx}+Be^{-ikx}$, Where $k=\frac{\sqrt{2m(E-V)}}{\hbar}$
- (E<V), Bounded , exponentially decaying and real 
	- $\phi = Ae^{k'x}+Be^{-ik'x}$, Where $k=\frac{\sqrt{2m(E-V)}}{\hbar}$


## Particle in a box
1D
- $\psi_n(x)=\sqrt{\frac{2}{a}}\sin \frac{n\pi x}{a}$
- $E_n=\frac{n^2\hbar^2\pi^2}{2ma^2}$
- $<x>=\frac{a}{2}$
- $<x^2>=a^2\left[\frac{1}{3}-\frac{1}{2n^2\pi^2}\right]$
	- $\Delta x =\sqrt{<x^2>-<x>^2}$
- $<p>=0$, for a real wave function 
- $<p^2>=\frac{n^2\hbar^2\pi^2}{a^2}$, from $\frac{p^2}{2m}=E_n$
	- $\Delta p = \frac{n^2\hbar^2\pi^2}{a^2}$ 

3D
- $\psi_n(x)=\sqrt{\frac{8}{abc}}\sin \frac{n_x\pi x}{a}\sin \frac{n_y\pi x}{b}\sin \frac{n_z\pi x}{c}$
- $E_{n_xn_yn_z}=\frac{\hbar^2\pi^2}{2m}\left(\frac{n^2_x}{a}+\frac{n^2_y}{b}+\frac{n^2_z}{c}\right)$

### symmetric potential  well
- $\psi_n(x)=\sqrt{\frac{2}{a}}\sin \frac{n\pi x}{a}$, for n= 2,4,6 odd wave function
- $\psi_n(x)=\sqrt{\frac{2}{a}}\cos \frac{n\pi x}{a}$, for n=1,2,3 even wave function
- $<x>=<p>=0$

## Step well potential
### $E>V_0$
- reflection coe $R=\frac{J_R}{J_I} = \left(\frac{k_1-k_2}{k_1+k_2}\right)^2= \left(\frac{p_1-p_2}{p_1+p_2}\right)^2$
- Transmission coe $T=\frac{J_T}{J_I} = 1-R=\frac{4k_1k_2}{(k_1+k_2)^2}= \frac{4p_1p_2}{(p_1+p_2)^2}$
	- $T+R=1$
	- $p=\hbar k$
	-  $J=\frac{\hbar}{2im}[\psi^*\nabla \psi - \psi \nabla \psi^*]$, J= probability current density 
### $E<V_0$
- $\psi=Ae^{ikx}+Be^{-ikx}$
	- $k^2=\frac{2mE}{\hbar^2}$
- $\psi_2=De^{-\alpha x}$
	- $\alpha^2 = \frac{2m(V_0-E)}{\hbar^2}$
## Finite square well potential
- $\eta=\zeta \tan \zeta$
- $\eta^2+\zeta^2=R$
	- $R=\frac{2mv_0}{\hbar^2}\text{(+ve width)}^2$
	- $\eta=\frac{k_1a}{2}$
	- $\zeta=\frac{k_2a}{2}$

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




